<div style="text-align:center"><img src=".assets/img/fluidos-banner.png" style="max-width: 60%;"/></div>


<p align="center">
  <a href="#bulb-about">About</a> &nbsp;&bull;&nbsp;
  <a href="#classical_building-the-fluidos-architecture">The Fluidos Architecture</a> &nbsp;&bull;&nbsp;
  <a href="#computer-click-and-play-playground">Click-and-play playground</a> &nbsp;&bull;&nbsp;
  <a href="#mag_right-research">Research</a> &nbsp;&bull;&nbsp;
  <a href="#toolbox-tech-stack">Tech Stack</a> &nbsp;&bull;&nbsp;
  <a href="#book-references-and-resources">Resources</a>
</p>

<br>

<div align="center">

|Service|Command Stack|
|---------------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:
| Node build      |          [![Node - Command Stack](https://github.com/fluidos-project/node/actions/workflows/build.yaml/badge.svg)](https://github.com/fluidos-project/node/actions/workflows/build.yaml)
| Node Artifacts     |          [![Node - Command Stack](https://github.com/fluidos-project/node/actions/workflows/check_artifacts.yaml/badge.svg)](https://github.com/fluidos-project/node/actions/workflows/check_artifacts.yaml)
| Node Helm Docs     |          [![Node - Command Stack](https://github.com/fluidos-project/node/actions/workflows/check-helm-documentation.yml/badge.svg)](https://github.com/fluidos-project/node/actions/workflows/check-helm-documentation.yml) 
| Node Linting    |          [![Node - Command Stack](https://github.com/fluidos-project/node/actions/workflows/lint.yaml/badge.svg)](https://github.com/fluidos-project/node/actions/workflows/lint.yaml) 
| Node Build Deployment    |          [![Node - Command Stack](https://github.com/fluidos-project/node/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/fluidos-project/node/actions/workflows/pages/pages-build-deployment) 


 :construction: <sub>Work in Progress (WIP)</sub>

</div>

 
## :bulb: About

The IT landscape has evolved into a world of hyperconnectivity, where devices and information systems communicate and exchange data on numerous applications. FLUIDOS will leverage the enormous, unused processing capacity at the edge, scattered across heterogeneous edge devices that struggle to integrate with each other and to form a seamless computing continuum coherently.

### :star: Give a Star! 

Support this research by **giving it a star**. Thanks!

## Documentation

The most up-to-date documentation about the project, the overall architecture, and the current implementation of the components is available in the [Docs](https://github.com/fluidos-project/Docs) repository.

## :classical_building: The Fluidos Architecture

### Fluidos Node
<div><img src=".assets/img/fluidos-node.png" style="max-width: 50%;"/></div>


## :desktop_computer: Software components

### Currently available components

<details>
    <summary> Fluidos Node </summary>

- A component that can consist of either a single device or a set of devices, primarily serving as a representation of a Kubernetes node. It is managed by a singular Kubernetes Control Plane. For additional information, kindly consult the [FLUIDOS node repository](https://github.com/fluidos-project/node)

</details>


<details>
    <summary> Fluidos at the edge</summary>

- FLUIDOS at the edge: a minimal architecture for running the FLUIDOS components at the edge of the network on some STM boards, leveraging KubeEdge.

</details>

### Current standalone components

<details>
    <summary> Cyber Deception </summary>

- A component to provide Cloud Native Cyber Deception as a service, thus enhancing the overall security of the FLUIDOS ecosystem. For additional information, kindly consult the [Cyber Deception repository](https://github.com/fluidos-project/cyber-deception)

</details>

## :computer: Click-and-play playground
This section summarizes the basic steps to reach a minimal setup of the available FLUIDOS components.

<details>
    <summary> Fluidos Node </summary>

### Fluidos Node

- Explore the FLUIDOS node with our step-by-step guide to effortlessly set up a FLUIDOS Node testbed using KIND (Kubernetes in Docker), which represents the simplest method to install this software on your local machine. [Begin your journey here.](https://github.com/fluidos-project/node/tree/main/testbed/kind)

</details>

<details>
    <summary> Fluidos at the edge </summary>

### Fluidos at the edge

- A minimal architecture for running the FLUIDOS components at the edge of the network on some STM boards, leveraging KubeEdge.

</details>


## :world_map: Roadmap