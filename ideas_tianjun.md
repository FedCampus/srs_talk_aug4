# Investigating Federated Learning Algorithms and Data Experiments under Non-IID Conditions

## Story Summary

I am a member of the algorithm group in the FedCampus team. A key point of
federated learning is to protect client data privacy, and the Federated Average
(FedAvg) algorithm provides a solution to this issue. However, there may be a
problem of non-independent and identically distributed (**non-IID**) data in
real data collection, i.e., the data distributions owned by different clients
are largely different.

My tests show that this significantly impacts the accuracy of the trained model
in the Federated Average algorithm. According to an analysis of the performance
of an MLP algorithm on a physical activity classifier dataset, the accuracy
drops from $$96\%$$ under **IID** distribution to $$57\%$$ under **non-IID**.

This issue is extremely important because, for FedCampus, it is very likely that
different clients' diverse lifestyles will generate differently distributed
data. Therefore, I have read more than ten Federated Learning algorithm papers
seeking solutions to this problem. Ultimately, in one algorithm (Federated
Learning via model distillation), the data accuracy under **non-IID** increased
from $$57\%$$ to over $$72\%$$.

### Experiment

I mainly conduct the experiments on the **DSA** (Daily and Sports Activities)
dataset. This dataset collects various sensor data, including speed and
pressure, at regular time intervals. My model's task is to predict what action
the tester is performing (for instance, squatting, walking, standing up, etc.)
based on these sensor data.

These experiements are conducted via light-weight models, with fixed training
rounds and epochs.

## Experiment Results

### IID data Centralized Learning v.s. FedAvg

|                      | Linear Model | MLP | LSTM |
|----------------------|--------------|-----|------|
| Centralized Learning | 84%          | 96% | 98%  |
| Federated Averaging  | 82%          | 96% | 97%  |

### IID v.s. non-IID data in different Federated Learning Algorithm (using MLP)

|              | Federated Averaging | Federated Averaging with Restricted Softmax | Federated Learning via Model Distillation |
|--------------|---------------------|---------------------------------------------|-------------------------------------------|
| IID data     | 96%                 | 96%                                         |                                           |
| non-IID data | 57%                 | 57%, but gets higher converge speed         | 72%                                       |
