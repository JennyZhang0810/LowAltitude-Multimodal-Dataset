<p align="center">
  <img src="assets/4.2_GIT.png" width="80%">
</p>

<h1 align="center">UAIV: A Large-Scale Low-Altitude Multimodal Dataset for Urban Intelligence</h1>

<p align="center">
  <i>Multi-scenario · Multi-modal · Multi-condition · Real-world UAV Intelligence</i>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Paper-Under%20Review-blue">
  <img src="https://img.shields.io/badge/License-MIT-green">
  <img src="https://img.shields.io/badge/Status-Partial%20Release-yellow">
  <img src="https://img.shields.io/badge/Annotations-17B%2B-red">
  <img src="https://img.shields.io/badge/Python-3.8%2B-blue">
  <img src="https://img.shields.io/badge/PyTorch-1.10%2B-orange">
</p>

<p align="center">
  Jiening Zhang¹, Yangming Zhang¹, Pengwei Yang¹, Yupeng Gao¹, Xi Wu¹, Junyu Liu¹, <br>
  Guoqing Wang¹,²\*, Tianyu Li¹\*, Yang Yang¹,²
</p>

<p align="center">
  ¹ <em>School of Computer Science and Engineering, University of Electronic Science and Technology of China</em><br>
  ² <em>Sichuan Artificial Intelligence Institute</em><br>
  \* <em>Corresponding authors</em>
</p>

---

## 📖 Table of Contents

- [🔥 Visual Teaser](#-visual-teaser)
- [🔥 Overview](#-overview)
- [✨ Highlights](#-highlights)
- [📊 Dataset Overview](#-dataset-overview)
- [🧩 Task Definitions](#-task-definitions)
  - [1. Scene Understanding](#1-scene-understanding)
  - [2. Spatio-Temporal Learning](#2-spatio-temporal-learning)
  - [3. Physics-Aware Image Restoration](#3-physics-aware-image-restoration)
- [🧪 Benchmark](#-benchmark-coming-soon)
- [📥 Data Access](#-data-access)
- [🚀 Applications & Real-World Impact](#-applications--real-world-impact)
- [📄 Dataset Description (Detailed)](#-dataset-description-detailed)
- [🙏 Acknowledgements](#-acknowledgements)
- [📚 Citation](#-citation)
- [📄 License](#-license)

---

## 🔥 Visual Teaser

<p align="center">
  <img src="assets/agricultural+commercial.png" width="45%">
  <img src="assets/burning+forest.png" width="45%">
</p>
<p align="center">
  <img src="assets/dark+IR.png" width="45%">
  <img src="assets/mining+pollution.png" width="45%">
</p>

---

## 🔥 Overview

**UAIV** is a large-scale low-altitude multimodal dataset designed for **urban intelligence and fine-grained governance analysis**, with a strong focus on:

- **Scene understanding**
- **Spatio-temporal reasoning**
- **Physics-aware image restoration**

Unlike conventional UAV datasets, UAIV emphasizes:

- **Cross-modal alignment** (RGB / IR / metadata)
- **Cross-view consistency**
- **Cross-condition robustness** (weather / illumination / viewpoint)

This enables models to learn **consistent and physically grounded representations** under real-world complexity.

The dataset is built upon a **self-operated UAV acquisition system**, covering **long-term, large-scale, real urban environments**, with strong diversity in:

- Scene types (urban / rural / industrial / natural)
- Illumination (day / night)
- Weather (rain / snow / fog / haze)
- Flight altitude and trajectories

---

## ✨ Highlights

- **17B+ high-quality annotations**
- **Cross-modal & cross-view alignment** (RGB / IR / metadata)
- **Multi-weather paired data** for restoration (rain / snow / fog)
- **Multi-temporal alignment** for change detection and Re-ID *(coming soon)*
- **Flexible UAV acquisition**: multi-altitude, multi-route, repeated sampling
- **Unified multi-task data paradigm** across perception, reasoning, and restoration
- **Object-level and scene-level consistency modeling**

---

## 📊 Dataset Overview

| Category | Details |
|----------|--------|
| Total Annotations | 17B+ |
| Scene Categories | urban, rural, forest, industrial, commercial, agricultural, residential, school, lake, etc. |
| Weather Conditions | sunny, rainy, foggy, snowy |
| Temporal Coverage | day, night |
| Modalities | RGB, IR, metadata (GPS, altitude, timestamp) |
| Flight Altitudes | 50m–500m |

---

## 🧩 Task Definitions

---

### 1. Scene Understanding

| Task | Input | Output | Key Challenge |
|------|-------|--------|---------------|
| Scene classification | RGB/IR | class label | cross-weather robustness |
| Semantic segmentation | RGB/IR | pixel mask | fine-grained urban elements |
| Instance segmentation | RGB/IR | instance masks | overlapping objects |
| Object counting | RGB/IR | count | scale variation |
| OCR | RGB | text | scene text under UAV view |
| Environment understanding | RGB/IR + metadata | semantic status | multi-modal reasoning |

**Description**

UAIV goes beyond conventional scene understanding benchmarks by emphasizing **context-rich and governance-oriented perception**. Each sample corresponds to **real urban governance scenarios**, such as illegal construction, open burning, environmental pollution, and infrastructure monitoring. The dataset provides **aligned multi-modal signals (RGB, IR, metadata)** and **strong environmental variations**, enabling models to jointly reason about object presence, scene semantics, and environmental status.

**Examples**

<p align="center">
  <img src="assets/agricultural+commercial.png" width="32%">
  <img src="assets/burning+forest.png" width="32%">
  <img src="assets/counting.png" width="32%">
</p>
<p align="center">
  <img src="assets/dark+IR.png" width="32%">
  <img src="assets/excavator+fire.png" width="32%">
  <img src="assets/farmland+excavation.png" width="32%">
</p>
<p align="center">
  <img src="assets/lake+forest.png" width="32%">
  <img src="assets/mining+pollution.png" width="32%">
  <img src="assets/OCR.png" width="32%">
</p>
<p align="center">
  <img src="assets/river_pollution.png" width="45%">
</p>

---

### 2. Spatio-Temporal Learning

| Task | Input | Output | Key Challenge |
|------|-------|--------|---------------|
| Change detection | image pairs (t1, t2) | change mask | distinguishing semantic change vs. appearance variation |
| Cross-time Re-ID | object sequences across time | identity | domain shift across time/viewpoint/altitude |

**Description**

UAIV is specifically designed for **spatio-temporal reasoning under real-world dynamics**, with carefully aligned multi-temporal data collected across different time spans, flight routes, and environmental conditions. For **change detection**, the dataset provides strictly aligned image pairs with variations in season, construction progress, and environmental status, allowing models to distinguish true semantic changes from appearance variations caused by illumination or weather. For **cross-time Re-ID**, UAIV introduces a challenging setting where objects (vehicles, ships, infrastructure) are observed across different timestamps, viewpoints, and altitudes, enabling research on identity-consistent representation learning under drastic domain shifts.

**Examples**

<p align="center">
  <img src="assets/Change_detection.png" width="45%">
  <img src="assets/re-id.png" width="45%">
</p>

---

### 3. Physics-Aware Image Restoration

| Task | Input | Output | Key Challenge |
|------|-------|--------|---------------|
| Rain removal | rainy RGB | clean RGB | real rain streaks, non-uniform |
| Snow removal | snowy RGB | clean RGB | occlusion, lighting change |
| Fog removal | foggy RGB | clean RGB | depth-dependent scattering |
| Cross-weather translation | degraded image | clear image | preserving scene content |

**Description**

Unlike synthetic benchmarks, UAIV provides **real-world paired and unpaired weather-degraded data**, including rain, snow, fog, and haze, captured under consistent UAV trajectories and sensor settings. The dataset preserves physical consistency across conditions (illumination variation, atmospheric scattering, sensor response differences), enabling the study of **physics-aware restoration** that aims to recover intrinsic scene properties rather than only performing appearance translation. The availability of **cross-modal signals (RGB–IR)** further allows models to leverage complementary information, making UAIV a valuable testbed for multi-modal restoration and physically grounded image enhancement.

**Examples**

<p align="center">
  <img src="assets/foggy.png" width="45%">
  <img src="assets/haze&original.png" width="45%">
</p>
<p align="center">
  <img src="assets/rainy.png" width="45%">
  <img src="assets/snowy.png" width="45%">
</p>

---

## 🧪 Benchmark (Coming Soon)

We will provide standardized benchmarks and baselines for:

- Scene understanding  
- Change detection  
- Image restoration  

---

## 📥 Data Access

- **Current status**: Partially released  
- Open subset (~30%) will be released  
- Full dataset will be available in future versions  

👉 GitHub: [https://github.com/JennyZhang0810/LowAltitude-Multimodal-Dataset/tree/main](https://github.com/JennyZhang0810/LowAltitude-Multimodal-Dataset/tree/main)  
👉 Project Page: [https://jennyzhang0810.github.io/LowAltitude-Multimodal-Dataset/](https://jennyzhang0810.github.io/LowAltitude-Multimodal-Dataset/)

> **Note**: The dataset has been submitted to **ScienceDB (Journal of Image and Graphics dataset track)** and is currently under review. The official data access link will be released after acceptance.

---

## 🚀 Applications & Real-World Impact

The dataset has been **deployed in real-world urban governance systems** using **Xuzhou (Jiangsu Province, China)** as a pilot region, and has achieved **full coverage of the Huaihai Economic Zone**.

Based on UAIV, we have developed:

- **21 domain-specific intelligent agents** for urban governance
- A **regional integrated government service platform**

The system supports automated analysis for:

- Illegal construction detection  
- Environmental anomaly monitoring  
- Infrastructure status assessment  

**Impact**

- Significant improvement in **semantic understanding under complex conditions**
- Enhanced **event detection accuracy**
- Reduced **manual inspection costs**
- Faster **decision-making and response efficiency**

**User Feedback**

Practical deployments demonstrate that UAIV provides:

- Strong coverage of **complex real-world scenarios**
- Robust representation of **multi-scale objects**
- High-quality **semantic consistency**

making it a **reliable foundation for large-scale model training and deployment**.

---

## 📄 Dataset Description (Detailed)

UAIV is a large-scale multimodal dataset designed for **urban fine-grained governance and low-altitude remote sensing intelligence**.

- Total scale: **17B+ annotations**
- Built from **long-term UAV data collection**
- Covers **high-resolution, multi-scale, and dynamic environments**

The dataset systematically supports:

- Illegal construction detection  
- Environmental monitoring  
- Traffic infrastructure analysis  
- Construction activity understanding  

In addition to detection and segmentation, UAIV integrates:

- Change detection  
- Weather-degraded image restoration  
- Person/object re-identification (Re-ID)  

It further constructs **high-quality image–semantic alignment**, forming a **unified cross-task and cross-modal data paradigm**.

---

## 🙏 Acknowledgements

This dataset was **designed and led by the author**, covering the full pipeline of:

- Data acquisition  
- Data organization  
- Annotation system design  

We sincerely thank:

- **Xuzhou Transportation Control Group** for large-scale UAV data acquisition support  
- **Multi-modal Intelligence Group (MIG) at UESTC**, led by Prof. Guoqing Wang and Prof. Yang Yang, for valuable collaboration and technical support  

---

## 📚 Citation

If you find UAIV useful for your research, please cite:

```bibtex
@article{zhang2025uaiv,
  title={UAIV: A Large-Scale Low-Altitude Multimodal Dataset for Urban Intelligence},
  author={Zhang, Jiening and Zhang, Yangming and Yang, Pengwei and Gao, Yupeng and Wu, Xi and Liu, Junyu and Wang, Guoqing and Li, Tianyu and Yang, Yang},
  journal={arXiv preprint},
  year={2026}
}
