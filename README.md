<p align="center">
  <img src="assets/cover.png" width="80%">
</p>

---

## 🔥 Overview

**LAMD** is a large-scale, fully self-collected low-altitude multimodal dataset for **urban intelligence and ecological monitoring**, designed to support **unified modeling across perception, reasoning, and restoration tasks**.

Unlike existing UAV datasets, LAMD is built upon **real-world UAV flight acquisition**, with **strictly aligned multi-modal, multi-temporal, and cross-weather data**, enabling consistent learning under complex real environments.

A key feature of LAMD is its **reproducible data acquisition pipeline**:
- Fixed UAV flight routes  
- Multi-time & multi-weather re-capturing  
- Custom alignment & registration algorithms  

👉 Ensures **true spatial-temporal consistency instead of synthetic pairing**

---

## ✨ Core Characteristics

### 🔹 1. Fully Self-Collected & Reproducible UAV Data
- Manual UAV flights with fixed trajectories  
- Rich metadata:
  - GPS coordinates  
  - timestamps  
  - flight altitude  
  - camera parameters  

👉 Supports **trajectory-level analysis & reproducibility**

---

### 🔹 2. Cross-Modal & Cross-Condition Alignment 🔥
- RGB / Infrared / Metadata aligned  
- Cross-weather (rain / snow / fog / sunny)  
- Cross-time (day / night / seasonal)  
- Cross-view & multi-altitude  

👉 Enables:
- domain generalization  
- robust perception  
- physics-aware modeling  

---

### 🔹 3. Multi-Temporal Paired Data
- Same routes under different:
  - weather  
  - time  

👉 Supports:
- change detection  
- cross-time Re-ID  
- temporal reasoning  

**✔ Real-world paired data (NOT synthetic)**

---

### 🔹 4. Large-Scale Annotation
- 17B+ annotations  
- Semi-automatic + manual verification  
- Pixel / instance / event-level labels  

---

### 🔹 5. Physics-Aware Image Restoration 🌫️
- Fog / snow / rain degradation  
- Real captured weather effects  

👉 **NOT synthetic noise — real physical degradation process**

---

## 🖼️ Visual Examples

### 🏙️ Scene Understanding

<p align="center">
  <img src="assets/agricultural_commercial.png" width="45%">
  <img src="assets/burning_forest.png" width="45%">
</p>

<p align="center">
  <img src="assets/counting.png" width="45%">
  <img src="assets/dark_ir.png" width="45%">
</p>

<p align="center">
  <img src="assets/excavator_fire.png" width="45%">
  <img src="assets/farmland_excavation.png" width="45%">
</p>

<p align="center">
  <img src="assets/lake_forest.png" width="45%">
  <img src="assets/mining_pollution.png" width="45%">
</p>

<p align="center">
  <img src="assets/ocr.png" width="45%">
  <img src="assets/river_pollution.png" width="45%">
</p>

---

### 🔄 Spatio-Temporal Learning

<p align="center">
  <img src="assets/change_detection.png" width="60%">
</p>

<p align="center">
  <img src="assets/re_id.png" width="60%">
</p>

---

### 🌫️ Image Restoration (Real Degradation)

<p align="center">
  <img src="assets/foggy.png" width="45%">
  <img src="assets/haze_original.png" width="45%">
</p>
<p align="center">
  <em>Foggy input vs. clear condition (same trajectory)</em>
</p>

<p align="center">
  <img src="assets/rainy.png" width="45%">
  <img src="assets/snowy.png" width="45%">
</p>

---

## 📊 Dataset Tasks

### 🏙️ Urban Intelligence
- Scene understanding  
- OCR (day/night/IR)  
- Environment state recognition  
- Category-aware counting  
- Road / river segmentation  
- Event understanding  

### 🌱 Ecological Monitoring
- Illegal mining  
- River pollution  
- Straw burning  
- Farmland monitoring  

### 🔄 Re-Identification
- Cross-time UAV tracking  
- Same trajectory identity matching  

---

## 🧪 Benchmark (Coming Soon)

- Scene understanding  
- Change detection  
- Image restoration  

---

## 📥 Data Access

- Open subset (~30%) coming soon  
- Full dataset release planned  

---

## 🛣️ Roadmap

- [ ] Fine-grained annotations  
- [ ] Re-ID expansion  
- [ ] Language grounding  
- [ ] Benchmark leaderboard  

---

## 🙏 Acknowledgements

- Xuzhou Transportation Control Group  
- UESTC Future Media Research Center  

---

## 📄 License

MIT License
