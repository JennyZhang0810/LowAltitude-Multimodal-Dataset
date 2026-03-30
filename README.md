# Low-Altitude Multimodal Dataset (LAMD)

<p align="center">
  <img src="assets/cover.png" width="100%">
</p>

---

## 🔥 Overview

**LAMD** is a large-scale low-altitude multimodal dataset for **urban intelligence**, focusing on **scene understanding, spatio-temporal reasoning, and physics-aware image restoration**.

Unlike conventional UAV datasets, LAMD emphasizes **cross-modal, cross-view, and cross-condition alignment**, enabling models to learn consistent representations across **weather, time, and viewpoints**.

The dataset covers diverse environments including **urban, rural, industrial, and natural scenes**, with rich variations in **illumination, weather, and flight altitude**.

---

## ✨ Highlights

- **17B+ high-quality annotations**
- **Cross-modal & cross-view alignment** (RGB / IR / metadata)
- **Multi-weather paired data** for restoration (rain / snow / fog)
- **Multi-temporal alignment** for change detection and Re-ID *(coming soon)*
- **Flexible UAV acquisition**: multi-altitude, multi-route, repeated sampling
- **Object-level and scene-level consistency modeling**

---

## 📊 Dataset Overview

<p align="center">
  <img src="assets/overview.png" width="85%">
</p>

- **Scene diversity**: urban / rural / industrial / natural  
- **Weather conditions**: sunny / rainy / foggy / snowy  
- **Temporal coverage**: day / night  
- **Metadata support**: GPS, timestamp, altitude, camera parameters  

---

## 🧩 Task Definitions

### 1. Scene Understanding
<p align="center">
  <img src="assets/task_scene.png" width="80%">
</p>

- Scene classification  
- Semantic segmentation  
- Instance segmentation  
- Object counting  
- OCR  
- Environment understanding  

---
<p align="center">
  <img src="assets/agricultural+commercial.png" width="100%">
</p>
<p align="center">
  <img src="assets/burning+forest.png" width="100%">
</p>
<p align="center">
  <img src="assets/counting.png" width="100%">
</p>
<p align="center">
  <img src="assets/dark+IR.png" width="100%">
</p>
<p align="center">
  <img src="assets/excavator+fire.png" width="100%">
</p
<p align="center">
  <img src="assets/farmland+excavation.png" width="100%">
</p
<p align="center">
  <img src="assets/lake+forest.png" width="100%">
</p
<p align="center">
  <img src="assets/mining+pollution.png" width="100%">
</p
<p align="center">
  <img src="assets/OCR.png" width="100%">
</p
<p align="center">
  <img src="assets/river_pollution.png" width="100%">
</p

### 2. Spatio-Temporal Learning
<p align="center">
  <img src="assets/Change_detection.png" width="80%">
</p>
<p align="center">
  <img src="assets/re-id.png" width="80%">
</p>
- Change detection  
- Cross-time Re-ID *(coming soon)*  

---

### 3. Physics-Aware Image Restoration
<p align="center">
  <img src="assets/foggy.png" width="80%">
</p>
<p align="center">
  <img src="assets/haze&original.png" width="80%">
</p>
<p align="center">
  <img src="assets/rainy.png" width="80%">
</p>
<p align="center">
  <img src="assets/snowy.png" width="80%">
</p>

- Rain / snow / fog removal  
- Cross-weather image translation  
- Weather-aware degradation modeling  

---

## 🧪 Benchmark (Coming Soon)

We will provide standardized benchmarks and baselines for:

- Scene understanding  
- Change detection  
- Image restoration  

---

## 📥 Data Access

- Open subset (~30%) will be released  
- Full dataset will be available in future versions  

👉 ScienceDB: Coming Soon  
👉 Download script: Coming Soon  

---

## 🛣️ Roadmap

- [ ] Fine-grained annotations  
- [ ] Re-ID labels  
- [ ] Multi-modal extensions (text descriptions)  
- [ ] Benchmark expansion  

---

## 🙏 Acknowledgements

This dataset was **designed and led by the author**, covering the full pipeline of **data acquisition, organization, and annotation design**.

We sincerely thank:

- **Xuzhou Transportation Control Group** for their strong support in large-scale UAV data acquisition  
- **Future Media Research Center, University of Electronic Science and Technology of China (UESTC)** for valuable collaboration and technical assistance  

---

## 📄 License

MIT License
