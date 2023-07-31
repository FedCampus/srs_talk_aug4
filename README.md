# FedCampus: A Federated Learning & Federated Analytics Experiment on DKU Campus

## Motivation for FedCampus (Steven, 20s)

How do we learn from data generated on DKU campus, without collecting them?

(Ask audience for answers).

(This is exact what FedCampus aims to achieve).

## Introducing FedCampus (30s)

- Privacy-preserving data collection platform for smart campus.
    - Data analytics.
    - Benefits community.
- Edge devices: smartphones, smartwatches, IoTs.
- Systems development to provide research potentials.
    - Some of them we introduce next.
- Collaboration wanted.

(Remind the question).

## Steps to build up FedCampus

1. Federated Learning platform.
1. ML & FL algorithms.
1. User-facing app.

## Federated Learning platform

<!-- Promise that FL solves our problem. -->

### Introducing Federated Learning (FL) (1min)

- Local data & local ML training.
- Central server coordinate training and aggregate ML model.
- Analogy: the Federated Government.

### Why FL is the way forward (20s)

- Centralized ML invades privacy land.
- ML using privacy data is useful.
- FL solves this problem, especially mobile FL.

### FL example: Gboard in 2017 (20s)

Google's smart keyboard.

- Next word prediction.
- Train on user's phones when idle.

### Existing mobile FL solutions suck (20s)

- FLaaS: send data to proprietary cloud.
- Open source solutions: poor mobile support/ very basic.

### FedKit: on-demand mobile FL platform for FedCampus

- Self-hosted & open source.
- Persistent on-demand service.
- Server-side ML model swapping.
- Telemetry.

(Tech stack graph).

### FedKit FL process (1min)

1. ML model: app obtains `.tflite` model from backend.
1. Spawn Flower server: app requests backend.
1. Train: using Flower with gRPC connection.

## ML & FL algorithms

### Health data and privacy

- Tremendously useful yet sensitive use case.

### Case study: sleep efficiency prediction (Aicha)

### Dealing with non-IID-ness (Tianjun)

TODO: How does this fit in.

## User-facing app (Beilong)

TODO: Getting data from Huawei Health, etc.

### Physical infrastructure (Johnny)

TODO: We cannot have data safety using cloud.

## How you can engage with us

- We are looking for collaboration using FL.
- We are continuously looking for new members.
- We will soon be looking for participants in our experiments.
