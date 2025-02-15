<div style="text-align:center"><img src=".assets/img/fluidos-banner.png" style="max-width: 60%;"/></div>

<br>

<div align="center">

|Service|Command Stack|
|---------------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:
| Node build      |          [![Node - Command Stack](https://github.com/fluidos-project/node/actions/workflows/build.yaml/badge.svg)](https://github.com/fluidos-project/node/actions/workflows/build.yaml)
| Node Artifacts     |          [![Node - Command Stack](https://github.com/fluidos-project/node/actions/workflows/check_artifacts.yaml/badge.svg)](https://github.com/fluidos-project/node/actions/workflows/check_artifacts.yaml)
| Node Helm Docs     |          [![Node - Command Stack](https://github.com/fluidos-project/node/actions/workflows/check-helm-documentation.yml/badge.svg)](https://github.com/fluidos-project/node/actions/workflows/check-helm-documentation.yml)
| Node Linting    |          [![Node - Command Stack](https://github.com/fluidos-project/node/actions/workflows/lint.yaml/badge.svg)](https://github.com/fluidos-project/node/actions/workflows/lint.yaml)
| Node Build Deployment    |          [![Node - Command Stack](https://github.com/fluidos-project/node/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/fluidos-project/node/actions/workflows/pages/pages-build-deployment)

</div>


## :bulb: About

The IT landscape has evolved into a world of hyperconnectivity, where devices and information systems communicate and exchange data on numerous applications. FLUIDOS leverages the enormous, unused processing capacity available anywhere (edge devices, edge of the network, fog, cloud), scattered across devices, servers and cluster that struggle to integrate with each other and to form a seamless computing continuum.

### :star: Give a Star!

Support this research by **giving it a star**. Thanks!

## Documentation

The most up-to-date documentation about the project, the overall architecture, and the current implementation of the components is available in the [Docs](https://github.com/fluidos-project/Docs) repository.


## :desktop_computer: Software components (1st Release of the integrated MetaOS)

### Currently available components

<details>
    <summary> FLUIDOS Node </summary>

- A component that can consist of either a single device or a set of devices, primarily serving as a representation of a Kubernetes cluster. It is managed by a single Kubernetes Control Plane. For additional information, check the [FLUIDOS node repository](https://github.com/fluidos-project/node).

- [FLUIDOS Node 1st Release](https://github.com/fluidos-project/node/releases/tag/v0.0.3)

</details>


<details>
    <summary> FLUIDOS at the edge</summary>

- FLUIDOS at the edge: a minimal architecture for running the FLUIDOS components at the edge of the network on some STM boards, leveraging KubeEdge. For additional information, check the [FLUIDOS at the Edge repository](https://github.com/fluidos-project/fluidos-edge).

- [FLUIDOS at the edge 1st Release](https://github.com/fluidos-project/fluidos-edge/releases/tag/v0.1)

</details>

<details>
    <summary> FLUIDOS MetaOrchestration</summary>

- FLUIDOS meta-orchestration:
    This component provides functionality to perform intent-based meta orchestration of workloads within FLUIDOS continuum.
    The component relies on the functionality provided by the FLUIDOS node (see above) to perform resource discovery and acquisition.
    The project itself is extensible, allowing the definition of specific models, or rule/heuristics, for the orchestration of the deployed workloads. For additional information, check the [FLUIDOS model-based Meta Orchestration repository](https://github.com/fluidos-project/fluidos-modelbased-metaorchestrator/).

- [FLUIDOS meta-orchestration 1st Release](https://github.com/fluidos-project/fluidos-modelbased-metaorchestrator/releases/tag/v0.0.3)

</details>

<details>
    <summary> kubectl FLUIDOS plugin</summary>

- kubectl FLUIDOS plugin:
    This project provides an extension (plugin) to kubectl to seamlessly interact with FLUIDOS components, namely meta-orchestrator(s).
    The project is developed using Python, and it acts as a bridge between traditional kubernetes requests and the one processed by the model-based meta orchestrator.
    Note that the pluging also allows interaction with the MSPL-based meta-orchestrator, thus providing a developer a single tool for transparently interacting with the FLUIDOS components. For additional information, check the [kubectl FLUIDOS plugin](https://github.com/fluidos-project/kubectl-fluidos-plugin/).

- [kubectl FLUIDOS plugin 1st Release](https://github.com/fluidos-project/kubectl-fluidos-plugin/releases/tag/0.0.1)

</details>

<details>
    <summary> FLUIDOS Identity Management</summary>

- FLUIDOS Identity Management:
    This component consists in an Aries agent modified for use dp-abc cryptography combined with Hyperledger Fabric as VDR to provide a very powerful interface when working with DID's, issuing VCredentials or using smart contracts. 
    These tools will help to secure any scenario that may occur in FLUIDOS and bring us an API with which we can, among other things; issue VCredentials, create DIDs for FLUIDS entities, create Verifiable Presentations from VCredentials and verify said VCredentials/VPresentations. For additional information, check the [Fluidos Identity Management Aries Framework](https://github.com/fluidos-project/idm-fluidos-aries-framework-go).

- [FLUIDOS Identity Management 1st Release](https://github.com/fluidos-project/idm-fluidos-aries-framework-go/releases/tag/v.1.0.0)

</details>

### Current standalone components

<details>
    <summary> Cyber Deception </summary>

- A component to provide Cloud Native Cyber Deception as a service, thus enhancing the overall security of the FLUIDOS ecosystem. For additional information, check the [Cyber Deception repository](https://github.com/fluidos-project/cyber-deception).

- [Cyber Deception 1st Release](https://github.com/fluidos-project/cyber-deception/releases/tag/v0.0.1)

</details>

<details>
    <summary> Serverless Function</summary>

- We leverage [fission.io](https://fission.io/), a framework for serverless functions on Kubernetes, to seamlessly execute functions in a multi-cluster environment based on FLUIDOS (or Liqo). This enables developers to deploy lightweight, event-driven code that scales dynamically on demand. A detailed description of the installation steps is provided at page [Serverless in multi-cluster environment](https://github.com/fluidos-project/multi-cluster-serverless-functions).

</details>

## :computer: Click-and-play playground
This section summarizes the basic steps to reach a minimal setup of the available FLUIDOS components.

<details>
    <summary> Fluidos Node </summary>

### Fluidos Node

- You can set up a FLUIDOS Node testbed using KIND (Kubernetes in Docker), which represents the simplest method to install this software on your local machine. [Begin your journey here.](https://github.com/fluidos-project/node/tree/main/testbed/kind).

</details>

<details>
    <summary> Fluidos at the edge </summary>

### Fluidos at the edge

- A minimal architecture for running the FLUIDOS components at the edge of the network on some STM boards, leveraging KubeEdge.

</details>

<details>
    <summary> Fluidos Identity Management</summary>

### Fluidos Identity Management
- To build a functional demo of the component, check the following guide [Fluidos Identity Management Guideline](https://github.com/fluidos-project/idm-fluidos-aries-framework-go/blob/main/README.md).

</details>  


## :world_map: Roadmap

Jan 2025: Upgrade of the entire FLUIDOS meta OS to Liqo 1.0.
