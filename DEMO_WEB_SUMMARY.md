# 🌐 AgriShield AI Web Application — Master Architecture & System Documentation

The **AgriShield AI Web Application** is a multi-section precision agriculture decision support platform integrating **16 Crop Datasets**, **Dual AI Inference (YOLOv8/YOLOv9 + Deep CNN Grad-CAM++)**, **Faculty ML Performance Scores**, and **Live India Weather API Telemetry**.

> **Application Entry Point**: [`index.html`](file:///c:/Users/amrut/OneDrive/Desktop/Deep%20learning/demo%20web/index.html)  
> **Stylesheet**: [`styles.css`](file:///c:/Users/amrut/OneDrive/Desktop/Deep%20learning/demo%20web/styles.css)  
> **Logic Engine**: [`app.js`](file:///c:/Users/amrut/OneDrive/Desktop/Deep%20learning/demo%20web/app.js)

---

## 📌 System Navigation & Core Features

### 1️⃣ Dual AI Diagnostic Predictor (`#tab-predictor`)
* **Faculty Requirement — Dual Model Integration**:
  * **Model 1: YOLO (YOLOv8m / YOLOv9-Custom)**: Real-time object detection providing bounding-box lesion coordinates ($x, y, w, h$), confidence scores, and lesion count.
  * **Model 2: Deep CNN (MobileNetV2 / ResNet-50 / DenseNet121)**: Deep feature classification coupled with **Grad-CAM++ Explainable AI** visual heatmaps.
* **4-Crop Selector**: Interactive switching between **Tomato 🍅**, **Rice 🌾**, **Corn / Maize 🌽**, and **Wheat 🌾**.
* **Weather-Triggered Advisory**: Calculates Crop Weather Suitability Index ($0-100\%$) and generates a 4-Phase Precaution Protocol.

---

### 2️⃣ 16 Crop Datasets Hub (`#tab-datasets`)
Contains **4 distinct datasets for 4 major agricultural crops** curated from Indian Agricultural Research Institutes (ICAR, IIT Delhi, VIT Vellore) and global repositories:

| Crop | # | Dataset Title | Source Institution | Direct Repository Access Link |
| :-: | :-: | :--- | :--- | :--- |
| **Tomato** | 1 | PlantVillage Tomato Leaf Dataset | Penn State Univ & Kaggle | 🔗 [Open Link](https://www.kaggle.com/datasets/kaustubhb999/tomato-leaf-disease-dataset) |
| **Tomato** | 2 | PlantDoc Tomato Field Dataset | IIT Delhi Research Group | 🔗 [Open Link](https://github.com/pratikkayal/PlantDoc-Dataset) |
| **Tomato** | 3 | ICAR-IIHR Tomato Disease & Severity | ICAR-IIHR Bengaluru & Mendeley | 🔗 [Open Link](https://data.mendeley.com/datasets/tywbtsjrjv/1) |
| **Tomato** | 4 | Roboflow Tomato Detection Universe | Roboflow Community | 🔗 [Open Link](https://universe.roboflow.com/tomato-disease-detection/tomato-leaf-diseases-yolo) |
| **Rice** | 5 | ICAR-IARI Rice Blast & Blight Dataset | ICAR-IARI New Delhi & Kaggle | 🔗 [Open Link](https://www.kaggle.com/datasets/vaceron/rice-leaf-diseases-dataset) |
| **Rice** | 6 | Kaggle Rice Leaf Disease Dataset | Kaggle Data Science Community | 🔗 [Open Link](https://www.kaggle.com/datasets/prasunroy/natural-images) |
| **Rice** | 7 | UCI Rice Leaf Pathology Repository | UCI Machine Learning Repository | 🔗 [Open Link](https://archive.ics.uci.edu/ml/datasets) |
| **Rice** | 8 | PlantDoc Rice Field Dataset | IIT Delhi Research Group | 🔗 [Open Link](https://github.com/pratikkayal/PlantDoc-Dataset) |
| **Maize** | 9 | PlantVillage Maize/Corn Leaf Dataset | Penn State Univ & Kaggle | 🔗 [Open Link](https://www.kaggle.com/datasets/smaranjitghose/corn-or-maize-leaf-disease-dataset) |
| **Maize** | 10 | ICAR Haryana MaizeNet Field Dataset | CCS Haryana Ag Univ & NIT Kurukshetra | 🔗 [Open Link](https://www.kaggle.com/datasets/nidhiparashar/maizenet-haryana-dataset) |
| **Maize** | 11 | Kaggle Corn Leaf Blight & Rust | Kaggle Agricultural Community | 🔗 [Open Link](https://www.kaggle.com/datasets/alessandraschultz/corn-leaf-diseases) |
| **Maize** | 12 | Roboflow Maize Leaf Detection Universe | Roboflow Universe | 🔗 [Open Link](https://universe.roboflow.com/maize-detection/maize-diseases-yolo) |
| **Wheat** | 13 | ICAR-IIWBR Karnal Wheat Rust Dataset | ICAR-IIWBR Karnal & Mendeley | 🔗 [Open Link](https://data.mendeley.com/datasets/wheat-rust-karnal/1) |
| **Wheat** | 14 | WheatDisease-HRY Field Dataset | Punjab Agricultural University | 🔗 [Open Link](https://www.kaggle.com/datasets/shivanichoudhary/wheatdisease-hry) |
| **Wheat** | 15 | PlantDoc Wheat Leaf Field Dataset | IIT Delhi Research Group | 🔗 [Open Link](https://github.com/pratikkayal/PlantDoc-Dataset) |
| **Wheat** | 16 | Roboflow Wheat Rust Detection Universe | Roboflow Universe | 🔗 [Open Link](https://universe.roboflow.com/wheat-pathology/wheat-leaf-rust-yolo) |

---

### 3️⃣ Faculty Evaluation: ML Scores & Performance Matrix (`#tab-ml-scores`)
Empirical benchmark table comparing **YOLO Object Detectors** (YOLOv8m, YOLOv9-Custom) vs **Deep CNN Classifiers** (MobileNetV2, ResNet-50, DenseNet121, ViT-CGA, MaizeNet) across:
- **Accuracy (%)**
- **Precision (%)**
- **Recall (%)**
- **F1-Score (%)**
- **mAP@0.5 (%)**
- **Inference Latency (ms)**
- **Parameter Footprint (MB)**

---

### 4️⃣ Live India Regional Weather Tracker API (`#tab-weather`)
Live meteorological monitoring covering major Indian agricultural hubs (Nashik, Karnal, Guntur, Medak, Ludhiana, Pune) tracking Temperature, Relative Humidity, Rainfall, Wind Speed, and vector risk triggers.

---

## 🎨 Design & Aesthetic Standard

- **Human-Crafted 60/40 Aesthetic**: Custom dark slate theme (`#0b0f19`, `#131b2e`), zero neon AI tropes, fluid typography (`Plus Jakarta Sans` & `Outfit`), high-legibility cards, micro-interactions, and tabular data layouts.
- **Responsive**: Adapts fluidly across 4K monitors, laptops, tablets, and mobile devices.
