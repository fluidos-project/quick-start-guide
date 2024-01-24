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

### All Fluidos
![](https://raw.githubusercontent.com/fluidos-project/node)    

### Fluidos Node
![](https://raw.githubusercontent.com/fluidos-project)


## :desktop_computer: Software components
Currently available components:

- FLUIDOS node: a component that can consist of either a single device or a set of devices, primarily serving as a representation of a Kubernetes node. It is managed by a singular Kubernetes Control Plane. For additional information, kindly consult the [FLUIDOS node repository](https://github.com/fluidos-project/node)
- FLUIDOS at the edge: a minimal architecture for running the FLUIDOS components at the edge of the network on some STM boards, leveraging KubeEdge.


<details>
    <summary> Fluidos Node </summary>

-A component that can consist of either a single device or a set of devices, primarily serving as a representation of a Kubernetes node. It is managed by a singular Kubernetes Control Plane. For additional information, kindly consult the [FLUIDOS node repository](https://github.com/fluidos-project/node)

</details>


<details>
    <summary> Fluidos at the edge</summary>

-FLUIDOS at the edge: a minimal architecture for running the FLUIDOS components at the edge of the network on some STM boards, leveraging KubeEdge.

</details>

## :computer: Click-and-play playground
This section summarizes the basic steps to reach a minimal setup of the available FLUIDOS components.

<details>
    <summary> Fluidos Node </summary>

### Fluidos Node

-Explore the FLUIDOS node with our step-by-step guide to effortlessly set up a FLUIDOS Node testbed using KIND (Kubernetes in Docker), which represents the simplest method to install this software on your local machine. [Begin your journey here.](https://github.com/fluidos-project/node/tree/main/testbed/kind)

</details>

<details>
    <summary> Fluidos at the edge </summary>

### Fluidos at the edge

-A minimal architecture for running the FLUIDOS components at the edge of the network on some STM boards, leveraging KubeEdge.

</details>

<details>
    <summary> Fluidos Cybersecurity </summary>

### Fluidos Cybersecurity

Cybersecurity TODO

</details>


## :world_map: Roadmap

## :mag_right: Research

<details>
    <summary> Liquid computing </summary>

### Liquid computing

Liquid computing is a design approach...

</details>

## :rocket: Performance Evaluation

<details>
    <summary>FLUIDOS KPI's & Risks</summary>

### KPI

-Number of “base” OS supported: >= 4;  
TODO

</details>


## :computer: Running

Projects may have different environments where the application runs: development, staging, production, etc. Usually, different environments should have different settings.

<details>
    <summary>Development</summary>

### Development

// TODO
</details>

<details>
    <summary>Staging</summary>

### Staging

// TODO
</details>

<details>
    <summary>Production</summary>

### Production

// TODO

</details>

<details>
    <summary>Integration</summary>

### SECURITY INTEGRATION
// TODO
### NODE INTEGRATION
// TODO
</details>

## :test_tube: Tests

<details>
    <summary>Unit Tests</summary>

### Unit Tests

To unit-test an event-sourced aggregate, it's to verify that the Aggregate produces the expected event as output given a specific set of input Events and a Command. This involves creating an Aggregate
instance, applying the input events to it, handling the command, and verifying the expected event output.

```csharp
public void UnitTest()
```

</details>

<details>
    <summary>Integration Tests</summary>

### Integration Tests

// TODO

</details>

<details>
    <summary>Load Tests</summary>

### Load Testing (K6)

```bash
docker run --network=internal --name k6 --rm -i grafana/k6 run - <test.js
```

</details>

## :book: References and Resources

### Public Deliverables

- [D2.1 SCENARIOS, REQUIREMENTS AND REFERENCE ARCHITECTURE – V.1](https://www.fluidos.eu/wp-content/uploads/sites/86/2023/08/D2.1_v1.pdf)

### Books

- [Fluidos book](https://www.amazon.com/dp-0321125215/dp/0321125215/ref=mt_other?_encoding=UTF8&me=&qid=1641385448)


### Articles

- [A multi-layer guided reinforcement learning-based tasks offloading in edge computing](https://www.sciencedirect.com/science/article/pii/S1389128622005102)
- [Assessing the Potential Energy Savings of a Fluidified Infrastructure](https://ieeexplore.ieee.org/document/10132024)
- [Serverless computing: A security perspective](https://journalofcloudcomputing.springeropen.com/articles/10.1186/s13677-022-00347-w#citeas)
- [Locality-aware deployment of application microservices for multi-domain fog computing](https://linkinghub.elsevier.com/retrieve/pii/S0140366423000506)
- [By-default Security Orchestration on distributed Edge/Cloud Computing Framework](https://ieeexplore.ieee.org/document/10175478)
- [Enhancing Network Intrusion Detection: An Online Methodology for Performance Analysis](https://ieeexplore.ieee.org/document/10175465)
- [Computing Without Borders: The Way Towards Liquid Computing](https://ieeexplore.ieee.org/document/9984946)
- [Decentralised Identity Managementsolution for Zero-Trust Multi-domain Computing Continuum Frameworks(IN REVIEW)](https://um.es)

### Blogs

- [Fluidos consortium Blog](https://www.fluidos.eu/news-press-release-2/)


### Posts

- [How messaging simplifies and strengthens your microservice application - Callum Jackson](https://developer.ibm.com/articles/how-messaging-simplifies-strengthens-microservice-applications/)

### Projects (in progress)

- [Fluidos Node](https://github.com/fluidos-project/node)
- [Security](https://github.com/fluidos-project/security)

## :toolbox: Tech Stack

### Worker Services (in progress)

- [.NET 8](https://dotnet.microsoft.com/en-us/) - A free, multi/cross-platform and open-source framework;
- [MongoDB](https://www.mongodb.com/docs/drivers/csharp/) - A source-available cross-platform document-oriented database (Projections Database);


### Web API (in progress)

- [ASP.NET Core 8](https://devblogs.microsoft.com/dotnet/asp-net-core-updates-in-net-7-preview-1/) - A free, cross-platform and open-source web-development framework;

### Web APP (in progress)

- [Blazor WASM](https://docs.microsoft.com/en-us/aspnet/core/blazor/?WT.mc_id=dotnet-35129-website&view=aspnetcore-6.0#blazor-webassembly) - Is a single-page app (SPA) framework for building
  interactive client-side web apps with .NET;
- [BlazorStrap](https://blazorstrap.io/V5/) - Bootstrap 5 Components for Blazor Framework;

## Partners

<div style="text-align:center"><img src=".assets/img/partners.png" style="max-width: 60%;"/></div>

- [Martel innovate](https://www.martel-innovate.com/)
- [RSE](https://www.rse-web.it/)
- [Robotnik](https://robotnik.eu/)
- [ST](https://www.st.com/content/st_com/en.html)
- [Polito](https://www.polito.it/)
- [tu.berlin](https://www.tu.berlin/en/)
- [Helenic Mediterranean University](https://hmu.gr/en/home/)
- [Digital SME](https://www.digitalsme.eu/)
- [Fondazione Bruno Kessler](https://www.fbk.eu/en/)
- [Telefónica](https://www.telefonica.com/en/)
- [Borderstep Institute](https://www.borderstep.org/)
- [CYSEC](https://www.cysec.com/)
- [Terraviewos](https://www.terraview.co/)
- [Universidad De Murcia](https://www.um.es/)
- [Top-ix](https://www.top-ix.org/en/)
- [IBM](https://www.ibm.com/)


## Contributing

Contributions are welcome. Please take a look at [contributing](./CONTRIBUTING.md) guide.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/fluidos-project/tags).

## Authors

> See the list of [contributors](https://github.com/fluidos-project/general-activities/contributors) who participated in this project.

## License

This project is licensed under the BSD 3 License - see the [LICENSE](./LICENSE) file for details