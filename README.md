# FedCampus: A Federated Learning & Federated Analytics Experiment on DKU Campus

## TODO

- [ ] One problem to solve, as theme.
- [ ] FL application.
    - Gboard in 2017.
- [ ] Stress giving to the community.

## The FedCampus platform

### Motivation for FedCampus

How do we learn from data generated on DKU campus, without collecting them?

<!-- I am asking this question because this is exact what FedCampus aims to achieve. -->

### Introducing FedCampus (Steven, 30s)

- Privacy-preserving data collection platform for smart campus.
    - Data analytics.
    - Benefits community.
- Edge devices: smartphones, smartwatches, IoTs.
- Systems development to provide research potentials.
    - Some of them we introduce next.
    - Collaboration wanted.

<!-- Remind the question. -->

#### Steps to build up FedCampus

1. Federated Learning platform.
1. ML & FL algorithms.
1. User-facing app.

### Federated Learning platform

<!-- Promise that FL solves our problem. -->

#### Introducing Federated Learning (FL) (1min)

- Local data & local ML training.
- Central server coordinate training and aggregate ML model.
- Analogy: the Federated Government.

#### Why FL is the way forward (20s)

- Centralized ML invades privacy land.
- ML using privacy data is useful.
- FL solves this problem, especially mobile FL.

#### Existing mobile FL solutions suck (20s)

- FLaaS: send data to proprietary cloud.
- Open source solutions: poor mobile support/ very basic.

### Flower: FL framework (30s)

- gRPC: coordinate training & transmit ML model parameters.
    - Connection: bidirectional & alive information.
- Strategies: schedule training & aggregate ML model.

#### FedKit: on-demand mobile FL platform for FedCampus

- Persistent on-demand service.
- Server-side ML model swapping.
- Telemetry.

(Tech stack graph).

#### FedKit FL process (1min)

1. ML model: app obtains `.tflite` model from backend.
1. Spawn Flower server: app requests backend.
1. Train: using Flower with gRPC connection.

## FedCampus potential use cases

### Health data and privacy

- Tremendously useful yet sensitive use case.

### Case study: sleep efficiency prediction (Aicha)

### Dealing with non-IID-ness (Tianjun)

TODO: How does this fit in.

## Start of the FedCampus app (Beilong)

### Physical infrastructure (Johnny)

## How you can engage with us

- We are looking for collaboration using FL.
- We are continuously looking for new members.
- We will soon be looking for participants in our experiments.
