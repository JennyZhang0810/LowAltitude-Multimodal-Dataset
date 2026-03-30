<p align="center">
  <img src="assets/cover.png" width="100%">
</p>

---

## 🔥 Overview

**LAMD** is a large-scale, fully self-collected low-altitude multimodal dataset for **urban intelligence and ecological monitoring**, designed to support **unified modeling across perception, reasoning, and restoration tasks**.

Unlike existing UAV datasets, LAMD is built upon **real-world UAV flight acquisition**, with **strictly aligned multi-modal, multi-temporal, and cross-weather data**, enabling consistent learning under complex real environments.

A key feature of LAMD is its **reproducible data acquisition pipeline**, where all data are captured along **fixed flight routes under different time and weather conditions**, and further processed with **custom alignment and registration algorithms**.

---

## ✨ Core Characteristics

### 🔹 1. Fully Self-Collected & Reproducible UAV Data
- All data are captured via **manual UAV flights**
- Includes **flight metadata**:
  - GPS coordinates  
  - timestamps  
  - flight altitude  
  - camera parameters  
- Supports **reproducible data acquisition and trajectory-level analysis**

---

### 🔹 2. Cross-Modal & Cross-Condition Alignment🔥
- RGB / Infrared (IR) / Metadata aligned
- Cross-weather alignment (rain / snow / fog / sunny)
- Cross-time alignment (day / night / seasonal)
- Cross-view & multi-altitude consistency
- Custom **registration algorithm** ensures spatial alignment

👉 Enables:
- domain generalization  
- robust perception  
- physics-aware modeling  

---

### 🔹 3. Multi-Temporal Paired Data
- Same flight routes under:
  - different weather  
  - different time  
- Naturally paired data for:
  - change detection  
  - cross-time Re-ID  
  - temporal reasoning  

👉 This is **NOT synthetic pairing**, but real-world aligned acquisition.

---

### 🔹 4. Large-Scale High-Quality Annotation
- **17B+ annotations**
- Semi-automatic annotation + manual verification
- Pixel-level + instance-level + event-level labels
- All images are paired with corresponding annotation files

---

### 🔹 5. High-Resolution & Multi-View Data
- High-resolution UAV imagery
- Large spatial coverage
- Multi-altitude capture
- Multi-perspective observation

---

## 📊 Dataset Structure

### 🏙️ Urban Intelligence

- **Scene Understanding**
  - Construction sites  
  - Industrial parks  
  - Transportation hubs  
  - Residential areas  
  - Agricultural land  
  - Commercial districts  
  - School zones  

- **OCR (Optical Character Recognition)**
  - Night (with IR)  
  - Sunny  
  - Rainy  

- **Environment State Recognition**

- **Category-aware Counting**
  - Ships  
  - Non-motor vehicles  
  - Street vendors  
  - Pedestrians  

- **Segmentation Tasks**
  - Road segmentation  
  - River segmentation  

- **Event Understanding**
  - River pollution  
  - Burning events  
  - Excavator operations  

---

### 🌱 Ecological Monitoring

- Illegal mining  
- River pollution  
- Lake water monitoring  
- Straw burning  
- Farmland monitoring  
- Excavation activities  

---

### 🔄 Re-Identification (Re-ID)

- Multi-temporal UAV tracking data  
- Same trajectory under different timestamps  
- Supports cross-time identity matching  

*(Ongoing expansion)*

---

### 🌫️ Physics-Aware Image Restoration

- Fog removal (paired data)  
- Snow degradation (video sequences)  
- Rain degradation (image-level)  

👉 Real captured degradation instead of synthetic noise

---

## 🖼️ Visual Examples

### Scene Understanding
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
</p>
<p align="center">
  <img src="assets/farmland+excavation.png" width="100%">
</p>
<p align="center">
  <img src="assets/lake+forest.png" width="100%">
</p>
<p align="center">
  <img src="assets/mining+pollution.png" width="100%">
</p>
<p align="center">
  <img src="assets/OCR.png" width="100%">
</p>
<p align="center">
  <img src="assets/river_pollution.png" width="100%">
</p>

---

### Spatio-Temporal Learning
<p align="center">
  <img src="assets/Change_detection.png" width="80%">
</p>
<p align="center">
  <img src="assets/re-id.png" width="80%">
</p>

---

### Image Restoration
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

---

## 🧪 Benchmark (Coming Soon)

We will provide standardized benchmarks for:

- Scene understanding  : Coming Soon 
- Change detection  : Coming Soon 
- Image restoration  : Coming Soon 

---

## 📥 Data Access

- Open subset (~30%) will be released  
- Full dataset available in future versions  

👉 ScienceDB: Coming Soon  
👉 Download tools: Coming Soon  

---

## 🛣️ Roadmap

- [ ] Fine-grained annotations  
- [ ] Re-ID labels expansion  
- [ ] Multi-modal extensions (text / language grounding)  
- [ ] Benchmark & leaderboard  

---

## 🙏 Acknowledgements

This dataset was **designed and led by the author**, covering the full pipeline of **UAV data acquisition, annotation system design, and dataset construction**.

We sincerely acknowledge:

- **Xuzhou Transportation Control Group** for their strong support in large-scale UAV data acquisition  
- **Future Media Research Center, University of Electronic Science and Technology of China (UESTC)** for collaborative efforts and technical contributions  

---

## 📄 License

MIT License
