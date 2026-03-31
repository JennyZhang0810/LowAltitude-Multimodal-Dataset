<p align="center">
  <img src="assets/GITHUB.png" width="90%">
</p>

<h1 align="center">UAIV: A Large-Scale Low-Altitude Multimodal Dataset for Urban Intelligence</h1>

<p align="center">
  <i>Multi-scenario • Multi-modal • Multi-condition • Real-world UAV Intelligence</i>
</p>

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

- **Scene diversity**: urban / rural / industrial / natural  
- **Weather conditions**: sunny / rainy / foggy / snowy  
- **Temporal coverage**: day / night  
- **Metadata support**: GPS, timestamp, altitude, camera parameters  

---

## 🧩 Task Definitions

---

### 1. Scene Understanding

**Tasks**
- Scene classification  
- Semantic segmentation  
- Instance segmentation  
- Object counting  
- OCR  
- Environment understanding  

**Description**

UAIV goes beyond conventional scene understanding benchmarks by emphasizing **context-rich and governance-oriented perception**.

Each sample is not only a visual recognition instance, but also corresponds to **real urban governance scenarios**, such as:

- Illegal construction
- Open burning
- Environmental pollution
- Infrastructure monitoring

Unlike static datasets, UAIV provides:

- **Aligned multi-modal signals (RGB, IR, metadata)**
- **Strong environmental variations**

This enables models to jointly reason about:

- Object presence
- Scene semantics
- Environmental status

making it particularly suitable for **robust perception under real-world uncertainty**.

---

**Examples**

<p align="center">
  <img src="assets/agricultural+commercial.png" width="45%">
  <img src="assets/burning+forest.png" width="45%">
</p>
<p align="center">
  <img src="assets/counting.png" width="45%">
  <img src="assets/dark+IR.png" width="45%">
</p>
<p align="center">
  <img src="assets/excavator+fire.png" width="45%">
  <img src="assets/farmland+excavation.png" width="45%">
</p>
<p align="center">
  <img src="assets/lake+forest.png" width="45%">
  <img src="assets/mining+pollution.png" width="45%">
</p>
<p align="center">
  <img src="assets/OCR.png" width="45%">
  <img src="assets/river_pollution.png" width="45%">
</p>

---

### 2. Spatio-Temporal Learning

**Tasks**
- Change detection  
- Cross-time Re-ID  

**Description**

UAIV is specifically designed for **spatio-temporal reasoning under real-world dynamics**, with carefully aligned multi-temporal data collected across:

- Different time spans  
- Flight routes  
- Environmental conditions  

For **change detection**, UAIV provides:

- **Strictly aligned image pairs**
- Variations in season, construction progress, and environmental status  

This allows models to distinguish:

- **True semantic changes**
- vs. **appearance variations caused by illumination or weather**

For **cross-time Re-ID**, UAIV introduces a challenging setting where objects (vehicles, ships, infrastructure) are observed across:

- Different timestamps  
- Viewpoints  
- Altitudes  

This enables research on **identity-consistent representation learning under drastic domain shifts**.

---

**Examples**

<p align="center">
  <img src="assets/Change_detection.png" width="45%">
  <img src="assets/re-id.png" width="45%">
</p>

---

### 3. Physics-Aware Image Restoration

**Tasks**
- Rain / snow / fog removal  
- Cross-weather image translation  
- Weather-aware degradation modeling  

**Description**

Unlike synthetic benchmarks, UAIV provides **real-world paired and unpaired weather-degraded data**, including:

- Rain  
- Snow  
- Fog  
- Haze  

captured under **consistent UAV trajectories and sensor settings**.

Crucially, the dataset preserves **physical consistency across conditions**, including:

- Illumination variation  
- Atmospheric scattering  
- Sensor response differences  

This enables the study of **physics-aware restoration**, aiming to recover:

- **Intrinsic scene properties**
rather than only performing appearance translation.

The availability of **cross-modal signals (RGB–IR)** further allows models to leverage complementary information, making UAIV a valuable testbed for:

- **Multi-modal restoration**
- **Physically grounded image enhancement**

---

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

👉 GitHub: https://github.com/JennyZhang0810/LowAltitude-Multimodal-Dataset/tree/main  
👉 Project Page: https://jennyzhang0810.github.io/LowAltitude-Multimodal-Dataset/  

> Note: The dataset has been submitted to **ScienceDB (Journal of Image and Graphics dataset track)** and is currently under review. The official data access link will be released after acceptance.

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

### Impact

- Significant improvement in **semantic understanding under complex conditions**
- Enhanced **event detection accuracy**
- Reduced **manual inspection costs**
- Faster **decision-making and response efficiency**

### User Feedback

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
- **Multi-modal Intelligence Group (MIG), UESTC** for valuable collaboration and technical support  

---

## 📄 License

MIT License
