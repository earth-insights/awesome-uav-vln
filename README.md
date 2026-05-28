<div align="center">

# 🚁 Awesome UAV-VLN

**A Curated Collection of Vision-Language Navigation for Unmanned Aerial Vehicles**

[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)
[![Papers](https://img.shields.io/badge/Papers-25%2B-0984e3?style=for-the-badge&logo=google-scholar&logoColor=white)](README.md)
[![Last Commit](https://img.shields.io/github/last-commit/earth-insights/awesome-uav-vln?style=for-the-badge&color=00b894)](https://github.com/earth-insights/awesome-uav-vln/commits)
[![Stars](https://img.shields.io/github/stars/earth-insights/awesome-uav-vln?style=for-the-badge&color=fdcb6e&logo=github)](https://github.com/earth-insights/awesome-uav-vln/stargazers)
[![Forks](https://img.shields.io/github/forks/earth-insights/awesome-uav-vln?style=for-the-badge&color=e17055&logo=github)](https://github.com/earth-insights/awesome-uav-vln/network/members)

<br>

*Organizing and showcasing state-of-the-art technologies in aerial robotics —*
*Vision-Language Navigation (VLN), Aerial Instruction Following, UAV-Environment Interaction,*
*and LLM-driven Drone Navigation.*

**We believe autonomous aerial navigation will experience its own "ChatGPT moment."**

<br>

---

</div>

## 📋 Table of Contents

| | Section | Description |
|:---:|:---|:---|
| 📚 | [Survey](#-survey) | Comprehensive surveys and reviews on UAV-VLN |
| 🚁 | [UAV-VLN Models](#-uav-vln-models) | Vision-Language Navigation for drones and aerial robots |
| 🧠 | [End-to-End UAV-VLN Models](#-end-to-end-uav-vln-models) |  Trainable models that directly map vision+language to actions |
| 🗺️ | [Semantic Cognitive Mapping & Zero Shot](#️-semantic-cognitive-mapping--zero-shot) |LLM/VLM-based semantic map construction for zero-shot UAV navigation |
| 📊 | [Benchmarks & Datasets](#-benchmarks--datasets) | Evaluation benchmarks & metrics for UAV-VLN |
| 🎮 | [Simulators](#-simulators) | Simulation platforms for aerial robots |
| 🔄 | [Sim-to-Real](#-sim-to-real) | Bridging simulation and real-world deployment |
| 🔗 | [Related Works](#-related-works) | Other awesome lists & related resources |

<br>

> [!NOTE]
> **Paper Ordering** — Within each year, papers are generally listed in reverse chronological order (newer papers appear lower). Particularly influential or representative works may be highlighted at the top regardless of date.

> [!TIP]
> **Contributing** — This repository is continuously updated! If you have papers, projects, or resources not yet included, please submit a **Pull Request** or open an **Issue**. Let's build a comprehensive resource for the aerial robotics and AI community!
>    
> **Entry Template:**
>```markdown
> - **[ShortName] Full Paper Title** - Author et al. *Conference Year*
>   - 📄 [Paper](link) | 💻 [Code](link) | 🎥 [Project](link)
>```


<br>

## 📚 Survey

> **Comprehensive surveys and review papers covering the landscape of uav-vln**
- [2026]Vision-Language Navigation for Aerial Robots:Towards the Era of Large Language Models
  - 📄[paper](https://arxiv.org/pdf/2604.07705)
- [2025]AeroVerse-Review: Comprehensive survey on aerial embodied vision-and-language navigation[[paper](https://arxiv.org/pdf/2408.15511)]
## 🚁 UAV-VLN Models
> **A complete collection of UAV-VLN methods**

### 2026
- **[NavDreamer]NavDreamer: Video Models as Zero-Shot 3D Navigators** - Huang et al. 
  - 📄 [Paper](https://arxiv.org/pdf/2602.09765) | 🌍 [Web](https://xinjiu612.github.io/NavDreamer)
  - 📝**Leverages video generation (Wan2.6) for future-view planning and \(\pi^3\) for trajectory waypoint extraction.**
  - 🔧 **Method**: Zero Shot | **Backbone**: Qwen-VL3

- **[OnFly]OnFly: Onboard Zero-Shot Aerial Vision-Language Navigation toward Safety and Efficiency** - Zheng et al. 
  - 📄 [Paper](https://arxiv.org/pdf/2603.10682v1) | 💻 [Code](https://github.com/Robotics-STAR-Lab/OnFly) 
  - 📝 **Leverages dual-agent decoupling, hybrid memory for progress monitoring, and semantic-geometric verification for safe goal refinement.**
  - 🔧 **Method**: Zero Shot | **Backbone**:Qwen3-VL-4B-AWQ |🌍 **Env**：UE4+Airsim

- **[AerialVLA] AerialVLA: A Vision-Language-Action Model for UAV Navigation via Minimalist End-to-End Control** - Xu et al. 
  - 📄 [Paper](https://arxiv.org/pdf/2603.14363) | 💻 [Code](https://github.com/XuPeng23/AerialVLA)
  - 🔧 **Method**: End-to-end | **Backbone**:OpenVLA |🌍 **Env**：OpenUAV

- **[AutoFly]AutoFly: Vision-Language-Action Model for UAV Autonomous Navigation in the Wild** - Sun et al. *ICLR 2026*
  - 📄 [Paper](https://arxiv.org/pdf/2602.09657) | 💻 [Code](https://github.com/xiaolousun/AutoFly-VLA)
  - 📝 **Integrates a pseudo-depth encoder to enhance spatial reasoning from RGB-only inputs for end-to-end VLA navigation.**
  - 🔧 **Method**: End-to-end | **Backbone**:LLaMA2-7B 

- **[Fly0]Fly0: Decoupling Semantic Grounding from Geometric Planning for Zero-Shot Aerial Navigation** - Xu et al.
  - 📄 [Paper](https://arxiv.org/pdf/2602.15875v1) |💻 [Code](https://github.com/xuzhenxing1/Fly0)
  - 📝 **Decouples MLLM-based semantic grounding from geometric planning, using 2D→3D projection and Ego-Planner for zero-shot aerial navigation.**
  - 🔧 **Method**: GSM

- **[AirHunt]AirHunt: Bridging VLM Semantics and Continuous Planning for Efficient Aerial Object Navigation** - Chen et al. 
  - 📄 [Paper](https://arxiv.org/pdf/2601.12742)

- **[APEX]APEX: A Decoupled Memory-based Explorer for Asynchronous Aerial Object Goal Navigation** - Zhang et al. *CVPR 2026*
  - 📄 [Paper](https://arxiv.org/pdf/2602.00551) | 💻 [Code](https://github.com/4amGodvzx/apex) 
  - **Employs a 3D dynamic spatio-semantic map with attraction, exploration, and obstacle channels, decoupled RL-based action decision, and parallel asynchronous execution for efficient aerial object goal navigation.**
  - 🔧 **Method**: GSM+RL

- **[IndoorUAV]IndoorUAV: Benchmarking Vision-Language UAV Navigation in Continuous Indoor Environments** - Liu et al. *AAAI 2026* 
  - 📄 [Paper](https://arxiv.org/pdf/2512.19024) |💻 [Code](https://github.com/valyentinee/IndoorUAV-Agent)|  📦 [Datasets](https://www.modelscope.cn/datasets/valyentine/Indoor_UAV) 

- **[OpenFly]Openfly: A comprehensive platform for aerial vision-language navigation** - Gao et al. *ICLR 2026*
  - 📄 [Paper](https://arxiv.org/pdf/2502.18041) | 💻 [Code](https://github.com/SHAILAB-IPEC/OpenFly-Platform) 
  - 📝 **First aerial VLN platform with automated data generation across multiple rendering engines and keyframe-aware agent.**
  - 🌍 **Env**:OpenFly | **Dataset**:OpenFly
  - 🔧 **Method**: End-to-end | **Action**:  Discrete: (DOF：4) | **Backbone**: Llama

- **[HETT] History-Enhanced Two-Stage Transformer for Aerial Vision-and-Language Navigation** -  Ding et al. *AAAI 2026*
  - 📄 [Paper](https://arxiv.org/pdf/2512.14222) | 💻 [Code](https://github.com/crotonyl/HETT)
  - 🔧 **Method**: End-to-end 
### 2025
- **[LongFly]LongFly: Long-Horizon UAV Vision-and-Language Navigation with Spatiotemporal Context Integration** - Jiang et al. *ICLR 2026*
  - 📄 [Paper](https://arxiv.org/pdf/2512.22010v1)

- **[See,Point,Fly] See, Point, Fly: A Learning-Free VLM Framework for Universal Unmanned Aerial Navigation** - Hu et al. *CoRL 2025*
  - 📄 [Paper](https://arxiv.org/pdf/2509.22653v1) | 💻 [Code](https://github.com/Hu-chih-yao/see-point-fly) 

- **[CityNavAgent] CityNavAgent: Aerial Vision-and-Language Navigation with Hierarchical Semantic Planning and Global Memory** - Zhang et al. *ACL 2025*
  - 📄 [Paper](https://arxiv.org/pdf/2505.05622) | 💻 [Code](https://github.com/EmbodiedCity/CityNavAgent.code) 

- **[CityNav] Vision-and-Language Navigation for UAVs** - Lee et al. *ICCV 2025*
  - 📄 [Paper](https://arxiv.org/pdf/2406.14240) | 💻 [Code](https://github.com/water-cookie/citynav) 
  - 📝 **First large-scale real-world dataset for aerial VLN.**
  - 🌍 **Env**:CityFlight  | **Dataset**: CityNav
  - 💡 **Novel**:Geographic Semantic Map
  
- **[OpenUAV]Towards Realistic UAV Vision-Language Navigation: Platform, Benchmark, and Methodology** - Wang et al. *ICLR 2025*
  - 📄 [Paper](https://arxiv.org/abs/2410.07087) | 💻 [Code](https://github.com/prince687028/TravelUAV) 
  - 📝 **UAV VLN platform featuring 6-DoF continuous trajectories, assistant-guided benchmark, and MLLM-based hierarchical navigation across 22 diverse scenes (urban, rural, forest, desert).**
  - 🔧 **Method**: End-to-end | **Action**: Discrete (DOF：4) | **Backbone**: Llama
  - 🌍 **Env**: AirSim + UE4 | **Dataset**:OpenUAV


- **[AeroDuo]AeroDuo: Aerial Duo for UAV-based Vision and Language Navigation** - Wu et al. *ACMM 2025*
  - 📄 [Paper](https://arxiv.org/pdf/2508.15232) | 💻 [Code](https://github.com/buaa-colalab/AeroDuo) 

### 2024
- **[NavAgent]NavAgent: Multi-scale Urban Street View Fusion For UAV Embodied Vision-and-Language Navigation** - Liu et al.
  - 📄 [Paper](https://arxiv.org/pdf/2411.08579)

- **[PIVOT]PIVOT: Iterative Visual Prompting Elicits Actionable Knowledge for VLMs** - Soroush et al. 
  - 📄 [Paper](https://arxiv.org/pdf/2402.07872) | 🌍 [Web](https://pivot-prompt.github.io/) 

- **[EmbodiedCity]EmbodiedCity: A Benchmark Platform for Embodied Agent in Real-world City Environment** - Gao et al. 
  - 📄 [Paper](https://arxiv.org/pdf/2410.09604)| 💻 [Code](https://github.com/tsinghua-fib-lab/EmbodiedCity) 

- **[TypeFly]TypeFly: Flying Drones with Large Language Model** - Chen et al. 
  - 📄 [Paper](https://arxiv.org/pdf/2312.14950) | 💻 [Code](https://github.com/typefly/TypeFly) 

### 2023

- **[AerialVLN] Vision-and-Language Navigation for UAVs** - Zhang et al. *ICCV 2023*
  - 📄 [Paper](https://arxiv.org/pdf/2308.06735) | 💻 [Code](https://github.com/AirVLN/AirVLN) 
  - 📝 **Proposes the first large-scale UAV-VLN benchmark, including simulator, dataset, and baselines.**
  - 🔧 **Method**: End-to-end | **Action**: Discrete (DOF：4) | **Backbone**: CMA
  - 🌍 **Env**: AirSim + UE4 | **Dataset**: AerialVLN/AerialVLN-S

- **[AVDN]Aerial Vision-and-Dialog Navigation** - Fan et al. *ACL 2023*
  - 📄 [Paper](https://arxiv.org/pdf/2205.12219) | 💻 [Code](https://sites.google.com/view/aerial-vision-and-dialog/home) 

## 🧠 End-to-End UAV-VLN Models
> **Trainable models that directly map vision+language to actions**

- **[AerialVLA] AerialVLA: A Vision-Language-Action Model for UAV Navigation via Minimalist End-to-End Control** - Xu et al. 
  - 📄 [Paper](https://arxiv.org/pdf/2603.14363) | 💻 [Code](https://github.com/XuPeng23/AerialVLA)

- **[AutoFly]AutoFly: Vision-Language-Action Model for UAV Autonomous Navigation in the Wild** - Sun et al. *ICLR 2026*
  - 📄 [Paper](https://arxiv.org/pdf/2602.09657) | 💻 [Code](https://github.com/xiaolousun/AutoFly-VLA) 

- **[APEX]APEX: A Decoupled Memory-based Explorer for Asynchronous Aerial Object Goal Navigation** - Zhang et al. *CVPR 2026*
  - 📄 [Paper](https://arxiv.org/pdf/2602.00551) | 💻 [Code](https://github.com/4amGodvzx/apex) 

- **[IndoorUAV]IndoorUAV: Benchmarking Vision-Language UAV Navigation in Continuous Indoor Environments** - Liu et al. *AAAI 2026* 
  - 📄 [Paper](https://arxiv.org/pdf/2512.19024) | 📦 [Datasets](https://www.modelscope.cn/datasets/valyentine/Indoor_UAV) | 💻 [Code](https://github.com/valyentinee/IndoorUAV-Agent)

- **[OpenFly]Openfly: A comprehensive platform for aerial vision-language navigation** - Gao et al. *ICLR 2026*
  - 📄 [Paper](https://arxiv.org/pdf/2502.18041) | 💻 [Code](https://github.com/SHAILAB-IPEC/OpenFly-Platform) 

- **[HETT] History-Enhanced Two-Stage Transformer for Aerial Vision-and-Language Navigation** -  Ding et al. *AAAI 2026*
  - 📄 [Paper](https://arxiv.org/pdf/2512.14222) | 💻 [Code](https://github.com/crotonyl/HETT)

- **[LongFly]LongFly: Long-Horizon UAV Vision-and-Language Navigation with Spatiotemporal Context Integration** - Jiang et al. *ICLR 2026*
  - 📄 [Paper](https://arxiv.org/pdf/2512.22010v1)

- **[CityNav] Vision-and-Language Navigation for UAVs** - Lee et al. *ICCV 2025*
  - 📄 [Paper](https://arxiv.org/pdf/2406.14240) | 💻 [Code](https://github.com/water-cookie/citynav) 

- **[OpenUAV]Towards Realistic UAV Vision-Language Navigation: Platform, Benchmark, and Methodology** - Wang et al. *ICLR 2025*
  - 📄 [Paper](https://arxiv.org/abs/2410.07087) | 💻 [Code](https://github.com/prince687028/TravelUAV) 

- **[AeroDuo]AeroDuo: Aerial Duo for UAV-based Vision and Language Navigation** - Wu et al. *ACMM 2025*
  - 📄 [Paper](https://arxiv.org/pdf/2508.15232) | 💻 [Code](https://github.com/buaa-colalab/AeroDuo) 

- **[NavAgent]NavAgent: Multi-scale Urban Street View Fusion For UAV Embodied Vision-and-Language Navigation** - Liu et al.
  - 📄 [Paper](https://arxiv.org/pdf/2411.08579)

- **[EmbodiedCity]EmbodiedCity: A Benchmark Platform for Embodied Agent in Real-world City Environment** - Gao et al. 
  - 📄 [Paper](https://arxiv.org/pdf/2410.09604)| 💻 [Code](https://github.com/tsinghua-fib-lab/EmbodiedCity) 

- **[AerialVLN] Vision-and-Language Navigation for UAVs** - Zhang et al. *ICCV 2023*
  - 📄 [Paper](https://arxiv.org/pdf/2308.06735) | 💻 [Code](https://github.com/AirVLN/AirVLN) 

- **[AVDN]Aerial Vision-and-Dialog Navigation** - Fan et al. *ACL 2023*
  - 📄 [Paper](https://arxiv.org/pdf/2205.12219) | 💻 [Code](https://sites.google.com/view/aerial-vision-and-dialog/home) 

## 🗺️ Semantic Cognitive Mapping & Zero Shot
> **Methods that explicitly build semantic-aware spatial representations or propose a pipeline for zero-shot or training-free navigation.**

- **[NavDreamer]NavDreamer: Video Models as Zero-Shot 3D Navigators** - Huang et al. 
  - 📄 [Paper](https://arxiv.org/pdf/2602.09765) 

- **[OnFly]OnFly: Onboard Zero-Shot Aerial Vision-Language Navigation toward Safety and Efficiency** - Zheng et al. 
  - 📄 [Paper](https://arxiv.org/pdf/2603.10682v1) | 💻 [Code](https://github.com/Robotics-STAR-Lab/OnFly) 

- **[Fly0]Fly0: Decoupling Semantic Grounding from Geometric Planning for Zero-Shot Aerial Navigation** - Xu et al.
  - 📄 [Paper](https://arxiv.org/pdf/2602.15875v1) |💻 [Code](https://github.com/xuzhenxing1/Fly0)

- **[AirHunt]AirHunt: Bridging VLM Semantics and Continuous Planning for Efficient Aerial Object Navigation** - Chen et al. 
  - 📄 [Paper](https://arxiv.org/pdf/2601.12742)

- **[See,Point,Fly] See, Point, Fly: A Learning-Free VLM Framework for Universal Unmanned Aerial Navigation** - Hu et al. *CoRL 2025*
  - 📄 [Paper](https://arxiv.org/pdf/2509.22653v1) | 💻 [Code](https://github.com/Hu-chih-yao/see-point-fly)

- **[CityNavAgent] CityNavAgent: Aerial Vision-and-Language Navigation with Hierarchical Semantic Planning and Global Memory** - Zhang et al. *ACL 2025*
  - 📄 [Paper](https://arxiv.org/pdf/2505.05622) | 💻 [Code](https://github.com/EmbodiedCity/CityNavAgent.code) 

- **[PIVOT]PIVOT: Iterative Visual Prompting Elicits Actionable Knowledge for VLMs** - Soroush et al. 
  - 📄 [Paper](https://arxiv.org/pdf/2402.07872) | 🌍 [Web](https://pivot-prompt.github.io/) 

- **[TypeFly]TypeFly: Flying Drones with Large Language Model** - Chen et al. 
  - 📄 [Paper](https://arxiv.org/pdf/2312.14950) | 💻 [Code](https://github.com/typefly/TypeFly) 

## 📊 Benchmarks & Datasets
> **Evaluation benchmarks and datasets specific to UAV-VLN.**
- **[OpenFly]Openfly: A comprehensive platform for aerial vision-language navigation** - Gao et al. *ICLR 2026*
  - 📄 [Paper](https://arxiv.org/pdf/2502.18041) | 💻 [Code](https://github.com/SHAILAB-IPEC/OpenFly-Platform) 

- **[CityNav] Vision-and-Language Navigation for UAVs** - Lee et al. *ICCV 2025*
  - 📄 [Paper](https://arxiv.org/pdf/2406.14240) | 💻 [Code](https://github.com/water-cookie/citynav) 

- **[OpenUAV]Towards Realistic UAV Vision-Language Navigation: Platform, Benchmark, and Methodology** - Wang et al. *ICLR 2025*
  - 📄 [Paper](https://arxiv.org/abs/2410.07087) | 💻 [Code](https://github.com/prince687028/TravelUAV) 

- **[AeroDuo]AeroDuo: Aerial Duo for UAV-based Vision and Language Navigation** - Wu et al. *ACMM 2025*
  - 📄 [Paper](https://arxiv.org/pdf/2508.15232) | 💻 [Code](https://github.com/buaa-colalab/AeroDuo) 

- **[EmbodiedCity]EmbodiedCity: A Benchmark Platform for Embodied Agent in Real-world City Environment** - Gao et al. 
  - 📄 [Paper](https://arxiv.org/pdf/2410.09604)| 💻 [Code](https://github.com/tsinghua-fib-lab/EmbodiedCity) 

- **[AerialVLN] Vision-and-Language Navigation for UAVs** - Zhang et al. *ICCV 2023*
  - 📄 [Paper](https://arxiv.org/pdf/2308.06735) | 💻 [Code](https://github.com/AirVLN/AirVLN) 

- **[AVDN]Aerial Vision-and-Dialog Navigation** - Fan et al. *ACL 2023*
  - 📄 [Paper](https://arxiv.org/pdf/2205.12219) | 💻 [Code](https://sites.google.com/view/aerial-vision-and-dialog/home) 

### 📦 Datasets
| Dataset | Environment | Scale | Instruction Granularity | Sensor | Type | Notes |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **[AerialVLN](https://www.kaggle.com/datasets/shuboliu/aerialvln)/[S](https://www.kaggle.com/datasets/shuboliu/aerialvln-s)** | 25 urban scenes | 8,446/3,916 | Step-by-step | RGB-D | Virtual | Early 3D, pilot traj |
| **[CityNav](https://github.com/water-cookie/citynav)** | Cambridge+Birm  |  32,637| Step-by-step | RGB-D | Real | human demo traj |
| **[OpenFly](https://huggingface.co/datasets/IPEC-COMMUNITY/OpenFly)** | 18 scenes | 100k |High-level | RGB-D,Lidar,PC | Real→Virtual | more engine, cross-scene |
| **[AVDN](https://sites.google.com/view/aerial-vision-and-dialog/home)** | Global satellite | 3,064  | Dialog-based / Mixed | RGB | Real | xView  satellite  |
| **[HaL-13k](https://modelscope.cn/datasets/Reynard/HaL-13k/files)** | OpenUAV | 13k |High-level  | RGB, LiDAR,PC | Virtual | Multi-UAV|
| **[OpenUAV](https://huggingface.co/datasets/wangxiangyu0814/TravelUAV)** | 22 diverse scenes  | 12k | Hybrid| RGB-D(5), LiDAR, IMU, GPS | Virtual |urban,rural,forest,desert|

> [!Note]
> - **Scale**: Number of trajectories.
> - **Instruction Type**: Level of instruction granularity
> - **Real/Virtual**: Virtual (simulation only) / Real (real-world captured) / Hybrid (both).
> - **Notes**: Licensing, access requirements, special features.

## 🎮 Simulators

> **Simulation platforms for aerial robot navigation and interaction.**

| Simulator | Virtual/Real | Engine | Environment | Key Features | Sensors |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **[AerialVLN](https://www.kaggle.com/datasets/shuboliu/aerialvln-simulators)** | Virtual | UE4 + AirSim | 25 urban scenes | First UAV-VLN sim, 870+ obj, 8 actions (4-DoF) | RGB-D |
| **[OpenUAV](https://huggingface.co/datasets/wangxiangyu0814/TravelUAV_env)** | Virtual | UE4 + AirSim | 22 suburban/natural | urban,rural,forest,desert, 6-DoF | RGB-D, IMU, GPS |Weather/lighting variations, complex dynamics | RGB, D, IMU |
| **[OpenFly](https://github.com/OpenFly)** | Real→Virtual | UE4/5, GTA-V, GE, 3DGS | 18 scenes, 150+ km² | Unified API, cross-scene generalization | RGB, D |
| **[CityNav](https://github.com/water-cookie/citynav)** | Real (recon) | WebGL (Potree) | Cambridge+Birm (8.7km²) | 3D recon, GSM | RGB, D (PC) |
| **[Embodied City](https://huggingface.co/datasets/EmbodiedCity/EmbodiedCity-Simulator)** | Real (recon) | UE5 + AirSim | Beijing CBD | Dynamic (pedestrians, vehicles), high detail | RGB,Depth,Segmentation,IMU,GPS |

> [!NOTE]
> - **Virtual**: Fully simulated environment (software only).
> - **Real**: Real-world platform or dataset (hardware involved).
> - **Real→Virtual**: Real-world data reconstructed into simulation.



## 🔄 Sim-to-Real
> **Techniques and case studies for transferring policies from simulation to real-world drones.**

<div align="center">

  <br>
  <details>
    <summary><b>📬 Help Wanted: Contribute Sim-to-Real Resources</b></summary>
    <br>
    <p>This area is currently under active development. If you know of relevant papers, projects, or case studies on <b>Sim-to-Real for UAV Vision-Language Navigation</b>, please consider contributing!</p>
    <ul>
      <li>📄 <b>Papers</b>: Any work addressing the gap between simulation and real-world drone deployment in language-guided navigation.</li>
      <li>🔧 <b>Techniques</b>: Domain randomization, sim-to-real adaptation, or system identification methods specifically for UAVs.</li>
      <li>🎥 <b>Real-world Demos</b>: Videos or open-source code repositories demonstrating successful real-world transfer.</li>
    </ul>
    <p>👉 Please submit via <a href="https://github.com/earth-insights/awesome-uav-vln/issues">Issue</a> or <b>Pull Request</b>. Thank you! 🙏</p>
  </details>
  <br>
</div>

## 🔗 Related Works

- [jonyzhang2023/awesome-embodied-vla-va-vln](https://github.com/jonyzhang2023/awesome-embodied-vla-va-vln)

- [Hub-Tian/UAVs_Meet_LLMs](https://github.com/Hub-Tian/UAVs_Meet_LLMs)

- [Sautenich/Awesome-Aerial-Vision-Language-Navigation](https://github.com/Sautenich/Awesome-Aerial-Vision-Language-Navigation)


- [Jiaaqiliu/Awesome-VLA-Robotics](https://github.com/Jiaaqiliu/Awesome-VLA-Robotics)

- [TheBrainLab/Awesome-VLA-UAVs](https://github.com/TheBrainLab/Awesome-VLA-UAVs)


---

<sub>
Built with ❤️ for the UAV-VLN community. <br>
Inspired by <a href="https://github.com/jonyzhang2023/awesome-embodied-vla-va-vln">Awesome Embodied VLA / VA / VLN</a>.
</sub>