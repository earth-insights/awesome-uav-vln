<div align="center">

# 🚁 Awesome UAV-VLN

**A Curated Collection of Vision-Language Navigation for Unmanned Aerial Vehicles**

[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)
[![Papers](https://img.shields.io/badge/Papers-10%2B-0984e3?style=for-the-badge&logo=google-scholar&logoColor=white)](README.md)
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
| 🗺️ | [Semantic Cognitive Mapping](#️-semantic-cognitive-mapping) |LLM/VLM-based semantic map construction for zero-shot UAV navigation |
| 📊 | [Benchmarks & Datasets](#-benchmarks--datasets) | Evaluation benchmarks & metrics for UAV-VLN |
| 🎮 | [Simulators](#-simulators) | Simulation platforms for aerial robots |
| 🔄 | [Sim-to-Real](#-sim-to-real) | Bridging simulation and real-world deployment |
| 🔗 | [Related Works](#-related-works) | Other awesome lists & related resources |

<br>

> [!NOTE]
> **Paper Ordering** — Within each year, papers are generally listed in reverse chronological order (newer papers appear lower). Particularly influential or representative works may be highlighted at the top regardless of date.

> [!TIP]
> **Contributing** — This repository is continuously updated! If you have papers, projects, or resources not yet included, please submit a **Pull Request** or open an **Issue**. Let's build a comprehensive resource for the aerial robotics and AI community!

<br>

## 📚 Survey

> **Comprehensive surveys and review papers covering the landscape of uav-vln**
- [2026]Vision-Language Navigation for Aerial Robots:Towards the Era of Large Language Models[[paper](https://arxiv.org/pdf/2604.07705)]
- [2025]AeroVerse-Review: Comprehensive survey on aerial embodied vision-and-language navigation[[paper](https://arxiv.org/pdf/2408.15511)]
## 🚁 UAV-VLN Models
> **A complete collection of UAV-VLN methods**

### 2026

### 2025

### 2024

### 2023
- **[AerialVLN] Vision-and-Language Navigation for UAVs** - Zhang et al. *ICCV 2023*📄 [Paper](https://arxiv.org/pdf/2308.06735) | 💻 [Code](https://github.com/AirVLN/AirVLN) 
  - 📝 **Proposes the first large-scale UAV-VLN benchmark, including simulator, dataset, and baselines.**
  - 🔧 **Method**: End-to-end | **Action**: Discrete (4-direction) | **Backbone**: ViT + LSTM
  - 🌍 **Env**: AirSim + UrbanCity | **Dataset**: UAV-Nav-10k


## 🧠 End-to-End UAV-VLN Models
> **Trainable models that directly map vision+language to actions**

## 🗺️ Semantic Cognitive Mapping
> **Methods that explicitly build semantic-aware spatial representations for zero-shot or training-free navigation.**

## 📊 Benchmarks & Datasets
> **Evaluation benchmarks and datasets specific to UAV-VLN.**

### 📦 Datasets
<table>
  <thead>
    <tr>
      <th width="15%">Dataset</th>
      <th width="15%">Environment</th>
      <th width="15%">Scale</th>
      <th width="18%">Instruction Type</th>
      <th width="12%">Sensor</th>
      <th width="12%">Real/Virtual</th>
      <th width="13%">Notes</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><b><a href="https://xxx">AerialVLN</a></b></td>
      <td>25 urban scenes (subway, factory, etc.)</td>
      <td>10k+ trajectories</td>
      <td>Step-by-step (long-horizon, 660+ steps avg)</td>
      <td>RGB, Depth</td>
      <td>Virtual (UE4 + AirSim)</td>
      <td>Early 3D dataset, professional pilot trajectories</td>
    </tr>
    <tr>
      <td><b><a href="https://xxx">CityNav</a></b></td>
      <td>Cambridge + Birmingham (8.7 km²)</td>
      <td>Large-scale human trajectories</td>
      <td>High-level (abstract city-scale tasks)</td>
      <td>RGB, Depth (point cloud)</td>
      <td>Real (reconstruction)</td>
      <td>Urban inspection, delivery scenarios</td>
    </tr>
    <tr>
      <td><b><a href="https://xxx">OpenFly</a></b></td>
      <td>18 real scenes, 150+ km²</td>
      <td>100k+ trajectories</td>
      <td>Synthetic (automatically generated)</td>
      <td>RGB</td>
      <td>Real (reconstruction)</td>
      <td>Low annotation cost, cross-scene generalization</td>
    </tr>
    <tr>
      <td><b><a href="https://xxx">AeroVerse</a></b></td>
      <td>Multiple (urban, suburban)</td>
      <td>500k+ (CyberAgent-Ego500k)</td>
      <td>Multi-level (scene, reason, nav, plan, act)</td>
      <td>RGB, Depth, IMU</td>
      <td>Virtual + Real</td>
      <td>5 downstream tasks, comprehensive benchmark</td>
    </tr>
    <tr>
      <td><b><a href="https://xxx">VDUAV</a></b></td>
      <td>Generic</td>
      <td>Not specified</td>
      <td><b>Multi-turn dialogue</b> (interactive)</td>
      <td>RGB</td>
      <td>Virtual</td>
      <td>Clarifies ambiguity, incremental instructions</td>
    </tr>
    <tr>
      <td><b><a href="https://xxx">RefDrone</a></b></td>
      <td>Cluttered 3D scenes</td>
      <td>Not specified</td>
      <td><b>Fine-grained spatial reasoning</b> (referential expressions)</td>
      <td>RGB, Depth</td>
      <td>Virtual</td>
      <td>Navigate to target by complex descriptions</td>
    </tr>
    <tr>
      <td><b><a href="https://xxx">UrbanVideo-Bench</a></b></td>
      <td>Urban</td>
      <td>Long-horizon trajectories</td>
      <td><b>Temporal dense caption</b> (video + nav)</td>
      <td>RGB</td>
      <td>Real (reconstruction)</td>
      <td>Combines navigation with video description</td>
    </tr>
    <tr>
      <td><b><a href="https://xxx">AVDN</a></b></td>
      <td>Global (satellite imagery)</td>
      <td>3,064 trajectories</td>
      <td>Multi-turn dialogue + attention data</td>
      <td>RGB (satellite)</td>
      <td>Real (satellite)</td>
      <td>Human-in-the-loop, attention distribution</td>
    </tr>
    <tr>
      <td><b><a href="https://xxx">UAV-VLPA-nano-30</a></b></td>
      <td>Urban, suburban, rural, natural</td>
      <td>30 satellite images</td>
      <td>High-level (abstract path planning)</td>
      <td>RGB (satellite, 1.5m/pixel)</td>
      <td>Real (satellite)</td>
      <td>Tests global VL understanding, 760m² per image</td>
    </tr>
    <tr>
      <td><b><a href="https://xxx">HaL-13k</a></b></td>
      <td>Mixed (multi-UAV coordination)</td>
      <td>13,000 pairs</td>
      <td>Hierarchical (high-level + low-level)</td>
      <td>RGB (aerial + ground)</td>
      <td>Virtual</td>
      <td>High-altitude + low-altitude UAV协同</td>
    </tr>
    <tr>
      <td><b><a href="https://xxx">UAV-VLN</a></b></td>
      <td>Satellite imagery</td>
      <td>Not specified</td>
      <td>Step-by-step (continuous point-to-point)</td>
      <td>RGB (satellite)</td>
      <td>Real (satellite)</td>
      <td>Pioneering benchmark for overhead navigation</td>
    </tr>
    <tr>
      <td><b><a href="https://xxx">OpenUAV</a></b></td>
      <td>100+ real-world locations</td>
      <td>Multiple per location</td>
      <td>Zero-shot / generalization (cross-scene)</td>
      <td>RGB, Depth, LiDAR, IMU, GPS</td>
      <td>Real (reconstruction)</td>
      <td>Tests robustness and zero-shot capability</td>
    </tr>
  </tbody>
</table>

> [!Note]
> - **Scale**: Number of trajectories / instruction pairs.
> - **Instruction Type**: Level of instruction granularity
> - **Real/Virtual**: Virtual (simulation only) / Real (real-world captured) / Hybrid (both).
> - **Notes**: Licensing, access requirements, special features.

## 🎮 Simulators

> **Simulation platforms for aerial robot navigation and interaction.**

<table>
  <thead>
    <tr>
      <th width="18%">Simulator</th>
      <th width="10%">Virtual / Real</th>
      <th width="15%">Engine</th>
      <th width="18%">Environment Type</th>
      <th width="22%">Key Features</th>
      <th width="17%">Sensor Suite</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><b><a href="https://github.com/AirVLN/AirVLN">Aerial VLN</a></b></td>
      <td>Virtual</td>
      <td>Unreal Engine 4 + AirSim</td>
      <td>25 urban scenes (subway, factory, etc.)</td>
      <td>First UAV-VLN simulator, 870+ object categories, 8 discrete actions (4-DoF)</td>
      <td>RGB, Depth</td>
    </tr>
    <tr>
      <td><b><a href="https://github.com/OpenUAV">OpenUAV</a></b></td>
      <td>Virtual</td>
      <td>Unreal Engine + CARLA</td>
      <td>22 suburban/rural/natural scenes</td>
      <td>Scene editing, dynamic environments, 6-DoF control</td>
      <td>RGB, Depth, IMU, LiDAR, GPS</td>
    </tr>
    <tr>
      <td><b><a href="https://github.com/UnrealZoo">UnrealZoo</a></b></td>
      <td>Virtual</td>
      <td>Unreal Engine + UnrealCV</td>
      <td>100 immersive scenes</td>
      <td>Open-world, 77 embodied agents (7 categories), discrete/continuous control</td>
      <td>RGB, Depth</td>
    </tr>
    <tr>
      <td><b><a href="https://github.com/AeroVerse/AeroSimulator">AeroSimulator</a></b></td>
      <td>Real (reconstruction)</td>
      <td>Unreal Engine</td>
      <td>Shanghai, Shenzhen (real cities)</td>
      <td>AeroVerse core, supports weather/lighting variations, complex flight dynamics</td>
      <td>RGB, Depth, IMU</td>
    </tr>
    <tr>
      <td><b><a href="https://github.com/OpenFly">OpenFly</a></b></td>
      <td>Real (reconstruction)</td>
      <td>UE4/5, GTA-V, Google Earth, 3D GS</td>
      <td>18 real scenes, 150+ km² (cities, campuses, historical)</td>
      <td>Unified API across engines, cross-scene generalization focus</td>
      <td>RGB, Depth</td>
    </tr>
    <tr>
      <td><b><a href="https://github.com/CityNav">CityNav</a></b></td>
      <td>Real (reconstruction)</td>
      <td>WebGL (Potree)</td>
      <td>Cambridge + Birmingham (8.7 km²)</td>
      <td>3D point cloud environment, 6-DoF flight control, structure-aware planning</td>
      <td>RGB, Depth (point cloud)</td>
     </tr>
    <tr>
      <td><b><a href="https://github.com/EmbodiedCity">Embodied City</a></b></td>
      <td>Real (reconstruction)</td>
      <td>Unreal Engine 5 + AirSim</td>
      <td>Beijing (CBD area)</td>
      <td>Dynamic elements (pedestrians, vehicles), high urban detail</td>
      <td>RGB, Depth, IMU</td>
     </tr>
    <tr>
      <td><b><a href="https://github.com/AVDN">AVDN</a></b></td>
      <td>Real (satellite)</td>
      <td>xView (2D)</td>
      <td>Global (satellite imagery)</td>
      <td>2D continuous navigation, coordinate-based movement, overhead perspective</td>
      <td>RGB (satellite)</td>
     </tr>
  </tbody>
</table>


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