<div style="text-align:center"><img src=".assets/img/fluidos-banner.png" style="max-width: 60%;"/></div>

<br>

<div align="center">

| Service               |                                                                                                      CI Status                                                                                                      |
| --------------------- | :-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
| Node build            |                   [![Node - Command Stack](https://github.com/fluidos-project/node/actions/workflows/build.yaml/badge.svg)](https://github.com/fluidos-project/node/actions/workflows/build.yaml)                   |
| Node Artifacts        |         [![Node - Command Stack](https://github.com/fluidos-project/node/actions/workflows/check_artifacts.yaml/badge.svg)](https://github.com/fluidos-project/node/actions/workflows/check_artifacts.yaml)         |
| Node Helm Docs        | [![Node - Command Stack](https://github.com/fluidos-project/node/actions/workflows/check-helm-documentation.yml/badge.svg)](https://github.com/fluidos-project/node/actions/workflows/check-helm-documentation.yml) |
| Node Linting          |                    [![Node - Command Stack](https://github.com/fluidos-project/node/actions/workflows/lint.yaml/badge.svg)](https://github.com/fluidos-project/node/actions/workflows/lint.yaml)                    |
| Node Build Deployment | [![Node - Command Stack](https://github.com/fluidos-project/node/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/fluidos-project/node/actions/workflows/pages/pages-build-deployment) |

</div>

## :bulb: About

The IT landscape is hyperconnected: devices and information systems continuously exchange data across edge, fog, and cloud. **FLUIDOS** taps into unused compute anywhere—edge devices, network edge, fog, and cloud—to create a seamless **computing continuum**.  
This repository collects quick-starts and links to the Release 2 components, playgrounds, and reproducible use cases.

### :star: Give a Star!

Support this research by **giving it a star**. Thanks!

## Documentation

The latest project-wide docs (architecture, concepts, and component guides) live in the **[Docs repository](https://github.com/fluidos-project/Docs)**.  
For hands-on setup, each component repo also includes quick-start instructions referenced below.

## :desktop_computer: Software components (Release 2 of the integrated MetaOS)

### Core components (Release 2)

<details>
  <summary> FLUIDOS Node </summary>

- Base component (one Kubernetes control plane per node) with **Broker** and **telemetry endpoint in REAR**, plus integration with **Liqo v1.0.0** for stable federation and peering.
- Repo: https://github.com/fluidos-project/node
</details>

<details>
  <summary> FLUIDOS Edge </summary>

- Minimal architecture for low-resource boards (e.g., STM) using **KubeEdge**, with documented layers (Cloud Core / Meta Edge / Deep Edge / Micro Edge).
- Repo: https://github.com/fluidos-project/fluidos-edge
</details>

<details>
  <summary> FLUIDOS MetaOrchestration </summary>

- **Model-based, intent-driven meta-orchestration**; clearer local vs. remote semantics, extended logging, Python 3.10 compatibility, and added tests.
- Repo: https://github.com/fluidos-project/fluidos-modelbased-metaorchestrator
</details>

<details>
  <summary> kubectl FLUIDOS plugin </summary>

- `kubectl` extension to interact with the model-based meta-orchestrator and MSPL-based paths.
- Repo: https://github.com/fluidos-project/kubectl-fluidos-plugin
</details>

<details>
  <summary> FLUIDOS Identity Management (PSM, DID/VC, JWT) </summary>

- **Privacy & Security Manager (PSM)** integrated with REAR: DID-backed JWT contracts (producer signs, consumer co-signs), VCs/VPs with p-ABC and ZKPs, XACML/ABAC via XADATU, PEP-proxied endpoints.
- Repo: https://github.com/fluidos-project/idm-fluidos-aries-framework-go
</details>

<details>
  <summary> FLUIDOS Cyber Deception (CDaaS) </summary>

- **Decepto**-based Cloud-Native Cyber Deception advertised via **FLAVOR** and activated by **intents/MSPL**; supports Meta-Orchestrator and Bastion flows, with an all-in-one testbed.
- Repo: https://github.com/fluidos-project/cyber-deception
</details>

<details>
  <summary> FLUIDOS Energy Predictors </summary>

- Daily node energy demand prediction (CNN), with dataset tooling and plotting helpers.
- Repo: https://github.com/fluidos-project/fluidos-energy-predictor
</details>

<details>
  <summary> Security Enhancements & Optional Features (WP5) </summary>

- Three security categories: **Integrated-by-Design (e.g., PSM)**, **Security Applications** (e.g., BeaCon, FLAD), and **Security Node Capabilities** (e.g., MAGI, TEE, Cyber Deception).
- Repo: https://github.com/fluidos-project/security-features
</details>

### New in Release 2

<details>
  <summary> FLUIDOS Node Dashboard </summary>

- **GUI** to browse/reserve/buy resources over **REAR**; deployed via Kubernetes manifests, exposed with **NodePort** services for backend/frontend.
- Repo: https://github.com/fluidos-project/fluidos-node-dashboard
</details>

<details>
  <summary> Telemetry & OpenTelemetry Collector </summary>

- Full observability stack: **kube-state-metrics**, **Node Exporter**, **OTEL Collector**, **Prometheus**, **Grafana**, **Alertmanager**; plus **plugin-api-otel** for dynamic OTEL pipeline management.
- Telemetry repo: https://github.com/fluidos-project/telemetry
- OTEL API repo: https://github.com/fluidos-project/plugin-api-otel
</details>

### Current standalone components

<details>
  <summary> Serverless Function </summary>

- Multi-cluster serverless with **Fission** on FLUIDOS/Liqo.
- Guide: https://github.com/fluidos-project/multi-cluster-serverless-functions
</details>

## :computer: Click-and-play playground

Quick paths to spin up minimal FLUIDOS setups on your machine or lab.

<details>
  <summary> FLUIDOS Node </summary>

### FLUIDOS Node

- Set up a FLUIDOS Node testbed using **KIND** (Kubernetes in Docker), the simplest local install path.  
 👉 [Begin here](https://github.com/fluidos-project/node/blob/main/docs/installation/installation.md).
</details>

<details>
  <summary> FLUIDOS at the Edge </summary>

### FLUIDOS at the Edge

- Minimal architecture to run FLUIDOS components on constrained boards (e.g., STM) using **KubeEdge**.  
 👉 [Project repo](https://github.com/fluidos-project/fluidos-edge).
</details>

<details>
  <summary> FLUIDOS Identity Management </summary>

### FLUIDOS Identity Management

- Build a functional demo with DIDs, Verifiable Credentials, and REAR integration.  
 👉 [Guideline](https://github.com/fluidos-project/idm-fluidos-aries-framework-go/blob/main/README.md).
</details>

<details>
  <summary> FLUIDOS Node Dashboard (Release 2) </summary>

### FLUIDOS Node Dashboard

- Web UI to browse, reserve, and purchase resources through **REAR**; deploy via Kubernetes manifests and expose via **NodePort** services.  
 👉 [Project repo](https://github.com/fluidos-project/fluidos-node-dashboard)
</details>

<details>
  <summary> Telemetry & OTEL Collector (Release 2) </summary>

### Telemetry & OTEL

- Observability stack (kube-state-metrics, Node Exporter, **OTEL Collector**, Prometheus, Grafana, Alertmanager) and **plugin API** to manage OTEL pipelines.  
 👉 Telemetry: https://github.com/fluidos-project/telemetry  
 👉 OTEL API: https://github.com/fluidos-project/plugin-api-otel
</details>

## :joystick: Playgrounds (integrated demonstrators)

The playgrounds are reproducible testbeds that integrate Node, Meta-Orchestrator, Identity/Security, and Observability, and capture KPI evidence.

- **FLUIDOS CoreNet (UMU)** — Security & privacy by design (PSM, DID/VC, REAR contracts and PEP-protected endpoints).  
  Repo: (see D9.3 for replication guide)

- **FLUIDOS LiveGrid (POLITO)** — Heterogeneous Cloud↔Edge continuum with centralized observability; validated on x86 and ARM (e.g., Tiesse routers); Edge→Cloud (LLM+GPU) and Cloud→Edge scenarios.  
  Repos: edge infra installer (POLITO), plus FLUIDOS Node

- **FLUIDOS FlexSim (FBK)** — Large-scale simulation (KWOK) integrating Node/Liqo/Meta-Orchestrator to stress-test scheduling and security.

- **FLUIDOS SmartCity (MARTEL)** — “Smart City in a box” pipeline showing FLUIDOS in a real urban scenario, with replication guidelines.

- **FLUIDOS Broker (TOPIX)** — Acts as a communication and routing hub where nodes can publish their announcements in order to make themselves visible to other participants in the FluidOS network.

- **FLUIDOS SensorFlow(HMU)** — Demonstrates node–edge–IoT integration by connecting cloud clusters with edge gateways and real IoT devices to enable end-to-end data acquisition, processing and secure sharing.

## :test_tube: Use cases (reproducible)

- **Intelligent Power Grid** — 3 FLUIDOS nodes; **PDC + Grid State Estimation** as FLUIDOSDeployments; **Percona XtraDB Cluster** (synchronous replication); Prometheus/Grafana dashboards; failure-injection scripts; automated K3s/FLUIDOS deployment.  
  Repo: https://github.com/fluidos-project/intelligent-power-grid-use-case

- **Smart Viticulture** — Offloading vineyard image processing to capable edge; provider/consumer setup scripts; image pipeline; packaged as **release v1.0.0**.  
  Repo: https://github.com/fluidos-project/smart-viticulture-uc

- **Robotic Logistics** — Dynamic offloading across robots/edge/cloud; orchestration modules and **FLUIDOS-RB-Theron** for execution/middleware; containerized components and automation to reproduce experiments.  
  Repos:  
  • https://github.com/fluidos-project/robotic-logistics-use-case  
  • https://github.com/fluidos-project/fluidos-rb-theron

## :world_map: Roadmap

- ✅ **Jan 2025**: Upgrade of the FLUIDOS MetaOS to **Liqo 1.0** (completed).
- ✅ **Oct 2025**: **Release 2** delivered (Node Dashboard, Telemetry/OTEL, R2 component updates, new playgrounds & reproducible use cases).
