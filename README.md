<p align="center">
  <img src="assets/cover.png" width="90%">
</p>

<h1 align="center">LAMD</h1>

<p align="center">
  <b>A Large-Scale Low-Altitude Multimodal Dataset for Urban Intelligence</b>
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

<p align="center">
  <i>Multi-scenario • Multi-modal • Multi-condition • Real-world UAV data</i>
</p>

---

## 🔥 Overview

**LAMD** is a large-scale low-altitude multimodal dataset for **urban intelligence**, focusing on **scene understanding, spatio-temporal reasoning, and physics-aware image restoration**.

Unlike conventional UAV datasets, LAMD emphasizes **cross-modal, cross-view, and cross-condition alignment**, enabling models to learn consistent representations across **weather, time, and viewpoints**.

The dataset covers diverse environments including **urban, rural, industrial, and natural scenes**, with rich variations in **illumination, weather, and flight altitude**.

---

## ✨ Highlights

<p align="center">

🚀 **17B+ high-quality annotations**  
🌐 **Cross-modal & cross-view alignment** (RGB / IR / metadata)  
🌧️ **Multi-weather paired data** for restoration (rain / snow / fog)  
🕒 **Multi-temporal alignment** for change detection and Re-ID *(coming soon)*  
✈️ **Flexible UAV acquisition**: multi-altitude, multi-route, repeated sampling  
🧠 **Object-level and scene-level consistency modeling**

</p>

---

## 📊 Dataset Overview

<p align="center">

**Scene diversity**  
urban / rural / industrial / natural  

**Weather conditions**  
sunny / rainy / foggy / snowy  

**Temporal coverage**  
day / night  

**Metadata support**  
GPS, timestamp, altitude, camera parameters  

</p>

---

## 🧩 Task Definitions

---

### 🏙️ 1. Scene Understanding

<p align="center">

Scene classification • Semantic segmentation • Instance segmentation  
Object counting • OCR • Environment understanding  

</p>

---

LAMD goes beyond conventional scene understanding benchmarks by emphasizing **context-rich and multi-condition perception**. Each example shown below is not only a standard visual recognition task, but also reflects **complex urban governance scenarios**, such as illegal excavation, open burning, environmental pollution, and infrastructure monitoring.

Unlike static datasets, LAMD provides **aligned multi-modal cues (RGB, IR, metadata)** and **diverse environmental variations**, enabling models to jointly reason about **object presence, scene semantics, and environmental status**. This makes it particularly suitable for studying **robust perception under real-world uncertainty**, where illumination, weather, and viewpoint continuously change.

---

<p align="center">
  <img src="assets/agricultural+commercial.png" width="60%">
</p>
<p align="center">
  <img src="assets/burning+forest.png" width="60%">
</p>
<p align="center">
  <img src="assets/counting.png" width="60%">
</p>
<p align="center">
  <img src="assets/dark+IR.png" width="60%">
</p>
<p align="center">
  <img src="assets/excavator+fire.png" width="60%">
</p>
<p align="center">
  <img src="assets/farmland+excavation.png" width="60%">
</p>
<p align="center">
  <img src="assets/lake+forest.png" width="60%">
</p>
<p align="center">
  <img src="assets/mining+pollution.png" width="60%">
</p>
<p align="center">
  <img src="assets/OCR.png" width="60%">
</p>
<p align="center">
  <img src="assets/river_pollution.png" width="60%">
</p>

---

### ⏳ 2. Spatio-Temporal Learning

<p align="center">

Change detection • Cross-time Re-ID  

</p>

---

LAMD is specifically designed to support **spatio-temporal reasoning under real-world dynamics**, with carefully aligned multi-temporal data collected across different time spans, flight routes, and environmental conditions.

For **change detection**, the dataset provides **strictly aligned image pairs** captured under varying conditions (e.g., seasonal changes, construction progress, environmental degradation), enabling models to distinguish **true semantic changes** from appearance variations caused by lighting or weather.

For **cross-time Re-ID**, LAMD introduces a unique setting where objects (e.g., vehicles, ships, infrastructure elements) are observed across **different timestamps, viewpoints, and altitudes**. This creates a challenging benchmark for learning **identity-consistent representations** under drastic changes in scale, orientation, and visual appearance.

These properties make LAMD particularly suitable for studying **long-term urban monitoring and dynamic scene understanding**, which are largely underexplored in existing UAV datasets.

---

<p align="center">
  <img src="assets/Change_detection.png" width="60%">
</p>
<p align="center">
  <img src="assets/re-id.png" width="60%">
</p>

---

### 🌦️ 3. Physics-Aware Image Restoration

---

Unlike synthetic degradation benchmarks, LAMD provides **real-world paired and unpaired data under diverse weather conditions**, including rain, snow, fog, and haze, captured with consistent flight trajectories and sensor settings.

Crucially, the dataset preserves **underlying physical consistency** across conditions, such as illumination changes, atmospheric scattering, and sensor response differences. This enables the study of **physics-aware restoration models** that go beyond appearance translation and instead recover **intrinsic scene properties**.

The availability of **cross-modal signals (e.g., RGB–IR pairs)** further allows models to leverage complementary information for restoration, making LAMD a valuable testbed for exploring **multi-modal and physically grounded image enhancement**.

---

<p align="center">
  <img src="assets/foggy.png" width="60%">
</p>
<p align="center">
  <img src="assets/haze&original.png" width="60%">
</p>
<p align="center">
  <img src="assets/rainy.png" width="60%">
</p>
<p align="center">
  <img src="assets/snowy.png" width="60%">
</p>

---

<p align="center">

Rain / snow / fog removal  
Cross-weather image translation  
Weather-aware degradation modeling  

</p>

---

## 🧪 Benchmark (Coming Soon)

<p align="center">

Scene understanding  
Change detection  
Image restoration  

</p>

---

## 📥 Data Access

<p align="center">

Open subset (~30%) will be released  
Full dataset will be available in future versions  

</p>

<p align="center">

👉 ScienceDB: Coming Soon  
👉 Download script: Coming Soon  

</p>

---

## 🙏 Acknowledgements

This dataset was **designed and led by the author**, covering the full pipeline of **data acquisition, organization, and annotation design**.

We sincerely thank:

- **Xuzhou Transportation Control Group** for their strong support in large-scale UAV data acquisition  
- **Future Media Research Center, University of Electronic Science and Technology of China (UESTC)** for valuable collaboration and technical assistance  

---

## 📄 License

MIT License
