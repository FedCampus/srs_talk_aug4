# SRS Presentation bullet points

- Presentation of myself; part of the algorithm team.
- What is federated learning? (one member of the team can present this)
- Working on sleep efficiency prediction, a task added to the FedCampus app. This task
    can be divided into two parts:
       - We can predict the efficiency of a night’s sleep based on the activity data of
    the same day. ***Mini-task I***
       - And, predict the sleep efficiency based on the activities and efficiency data
    of precious days (for example, based on the data of the past 6 days, we can predict
    what the sleep quality of a person would be in the 7 th day). ***Mini-task II – timeseries***
    ***data analysis***
- Data preprocessing was a big part of my work. I merged the online PMDataset set,
    that’s originally presented as inputs in different time ranges (each minute, hour, etc.)
    into one dataset containing the relevant features, and the final time duration type is
    days (the motive behind the choice of the dataset and the specific preprocessing
    methods can also be discussed)
- For both parts of the sleep efficiency task, I implemented algorithms using Keras-
    Tuner.
- For ***Mini-task I,*** our best model achieved a minimal mean absolute loss of 0.08 given
    the prediction range [0:100] (present the model)
- On the other hand, our best model for ***Mini-task II*** reached a loss of 0.1174 given the
    prediction range [0:100] (present the model). For both mini-tasks, further research
    can be done to decrease the loss.
- In addition to implementing these models, I researched different aggregation
    strategies on federated machine learning algorithms, mainly: FedAvg and FedProx,
    and was able to use them on our dataset... (I’ll run more tests using these algorithms
    and report the results in the presentation. I may also be able to add something about
    working with non-iid data).

During this research, I was able to learn many new skills including working with new libraries
like Tensorflow, Keras, Pytorch, reading and analyzing research papers on federated learning,
and deepening my knowledge of deep learning.
