# 🌊 Marine Oil Spill AI — AI-Driven Oil Spill Detection System

[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://5pxumguuwlteh5yqjscqsn.streamlit.app/)
![Python](https://img.shields.io/badge/Python-3.9+-blue?logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-Deep%20Learning-EE4C2C?logo=pytorch&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green)

> **Live Demo 🚀** → [https://5pxumguuwlteh5yqjscqsn.streamlit.app/](https://5pxumguuwlteh5yqjscqsn.streamlit.app/)

---

## 📖 About

**Marine Oil Spill AI** is an end-to-end deep learning system for detecting oil spills in satellite imagery. It uses a **U-Net** segmentation model trained on SAR (Synthetic Aperture Radar) satellite data to automatically identify and highlight oil-contaminated ocean regions.

This project was developed as part of the **AI SpillGuard OSD** program by **Kritika Sawhney**.

---

## ✨ Features

- 🛰️ **Satellite Image Analysis** — Upload any JPG/PNG satellite image for instant analysis
- 🤖 **U-Net Deep Learning Model** — State-of-the-art semantic segmentation architecture
- 🎯 **Oil Coverage Statistics** — Precise percentage coverage, pixel counts, and confidence scores
- 🚨 **Severity Classification** — Automatically classifies spills as MINIMAL / LOW / MODERATE / HIGH
- 🖼️ **Visual Overlay** — Color-coded overlay highlighting detected spill regions
- ⚡ **One-Click Detection** — Simple, user-friendly Streamlit interface

---

## 🖥️ Live App

👉 **[Click here to open the app](https://5pxumguuwlteh5yqjscqsn.streamlit.app/)**

Upload a satellite image → Click **Run AI Detection** → Get instant results!

---

## 🏗️ Project Structure

```
ML/
└── Kritika/
    ├── app.py                      # Streamlit web application
    ├── main.py                     # Core model logic
    ├── requirements.txt            # Python dependencies
    ├── runtime.txt                 # Python runtime version
    ├── oil_spill.ipynb             # Main training notebook
    ├── notebooks/
    │   ├── 00_dataset_overview.ipynb
    │   ├── 01_data_exploration.ipynb
    │   ├── 02_preprocessing.ipynb
    │   ├── 03_dataset_pipeline.ipynb
    │   ├── 04_model_development.ipynb
    │   ├── 05_train_oilspill_unet.ipynb
    │   └── 06_evaluation_and_visualisation.ipynb
    ├── results/
    │   ├── eda/
    │   ├── overview/
    │   └── preprocessing/
    ├── milestone_1_report.md       # Data Collection & Preprocessing
    ├── milestone_2_reports.md      # Model Development & Training
    └── milestone_final_report.md  # Evaluation, Deployment & Wrap-Up
```

---

## 🧠 Model Architecture

The project uses a **U-Net** convolutional neural network:

- **Encoder** — 4 downsampling blocks (64 → 128 → 256 → 512 channels)
- **Bottleneck** — 1024-channel feature map
- **Decoder** — 4 upsampling blocks with skip connections
- **Output** — Binary segmentation mask (oil / no oil)
- **Loss** — Binary Cross-Entropy + Dice Loss
- **Metrics** — IoU, Dice Score, Precision, Recall

---

## 📊 Milestones

| Milestone | Description | Status |
|-----------|-------------|--------|
| 1 | Data Collection & Preprocessing | ✅ Completed |
| 2 | Model Development & Training | ✅ Completed |
| 3 | Model Evaluation & Improvement | ✅ Completed |
| 4 | App Deployment & Project Wrap-Up | ✅ Completed |

---

## 🚀 Run Locally

```bash
# Clone the repository
git clone https://github.com/KritikaSawhney/ML.git
cd ML/ML/Kritika

# Install dependencies
pip install -r requirements.txt

# Run the Streamlit app
streamlit run app.py
```

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| Python | Core language |
| PyTorch | Deep learning framework |
| U-Net | Segmentation model architecture |
| Albumentations | Image augmentation |
| OpenCV | Image processing |
| Streamlit | Web app deployment |
| Google Drive | Model weights storage |

---

## 👩‍💻 Author

**Kritika Sawhney**
- GitHub: [@KritikaSawhney](https://github.com/KritikaSawhney)
- App: [Marine Oil Spill AI](https://5pxumguuwlteh5yqjscqsn.streamlit.app/)

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.
