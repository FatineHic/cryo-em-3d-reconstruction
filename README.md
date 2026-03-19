# 🔬 Cryo-EM Single Particle Analysis (SPA) Pipeline

**Full Single Particle Analysis workflow in cryo-electron microscopy, from raw particle images to 3D reconstruction and validation.**

[![Cryo-EM](https://img.shields.io/badge/Method-Cryo--EM-blueviolet)]()
[![SPA](https://img.shields.io/badge/Pipeline-SPA-blue)]()
[![Chimera](https://img.shields.io/badge/Viz-Chimera-green)]()
[![Structural Biology](https://img.shields.io/badge/Field-Structural_Biology-orange)]()

---

## 📌 Table of Contents

- [Overview](#-overview)
- [Objectives](#-objectives)
- [Workflow](#%EF%B8%8F-workflow)
- [Key Processing Steps](#-key-processing-steps)
- [Results](#-results)
- [Project Structure](#-project-structure)
- [Tools & Technologies](#%EF%B8%8F-tools--technologies)
- [Conclusion](#-conclusion)
- [Future Work](#-future-work)

---

## 🔬 Overview

This project demonstrates a **complete Single Particle Analysis (SPA) workflow** in cryo-electron microscopy. The pipeline covers every stage from raw particle images through alignment and classification to final 3D reconstruction and validation.

Cryo-EM SPA is a powerful technique for determining the **3D structure of biological macromolecules** at near-atomic resolution, without the need for crystallization.

---

## 🎯 Objectives

- Process particle images from cryo-EM data
- Perform alignment and classification (2D & 3D)
- Generate and refine 3D structures
- Validate reconstruction quality

---

## ⚙️ Workflow

```
Biological Sample
       │
       ▼
┌──────────────────────┐
│ 1. Sample Preparation│──→ Purification & vitrification
│                      │    Native structure in vitreous ice
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│ 2. Data Acquisition  │──→ Thousands of particle projections (TEM)
│                      │    Defocus, contrast, electron dose control
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│ 3. Particle Picking  │──→ Computational particle identification
│    & Extraction      │    Boxing, masking, extraction
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│ 4. Alignment &       │──→ 2D classification
│    Classification    │    3D classification
│                      │    High-quality class selection
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│ 5. 3D Reconstruction │──→ Ab initio model generation
│                      │    Iterative alignment refinement
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│ 6. Model Refinement  │──→ Symmetry constraints
│    & Validation      │    Real-space refinement
│                      │    Reprojection validation
└──────────────────────┘
           │
           ▼
   ✅ Validated 3D Structure
```

---

### 1. Sample Preparation

- Purification and vitrification of biological samples
- Preservation of native structure in vitreous ice

---

### 2. Data Acquisition

- Captured thousands of particle projections using **Transmission Electron Microscopy (TEM)**
- Controlled parameters: defocus, contrast, electron dose

---

### 3. Particle Picking & Extraction

- Identified particles using computational methods
- Extracted particles into boxed images
- Applied masking to focus on relevant regions

---

### 4. Alignment & Classification

- Aligned particles to a common reference
- Performed **2D classification** and **3D classification**
- Selected high-quality classes for reconstruction

---

### 5. 3D Reconstruction

- Generated initial 3D model (**ab initio**)
- Refined using iterative alignment

---

### 6. Model Refinement & Validation

- Improved structure using symmetry constraints and real-space refinement
- Validated results with reprojections

---

## 📊 Key Processing Steps

| Step | Description |
|:---|:---|
| **Bandpass filtering** | Remove noise from particle images |
| **Particle centering** | Alignment algorithms for accurate positioning |
| **MSA** | Multivariate Statistical Analysis for dimensionality reduction |
| **HAC** | Hierarchical Ascendant Classification for grouping |
| **Angular reconstitution** | Euler angle determination for 3D geometry |
| **Sinogram validation** | Verification of angular assignments |
| **MRA** | Multi-Reference Alignment for iterative improvement |

---

## 📈 Results

Successfully reconstructed two 3D models:

| Model | Status |
|:---|:---|
| `3d_0-1` | ✅ Reconstructed |
| `3d_0-2` | ✅ Reconstructed |

- Improved alignment and consistency with additional views
- Final models visualized in **Chimera**

---

## 📂 Project Structure

```
cryo-em-project/
│
├── report/                 # Project report
│   └── cryo_em_report.pdf
│
├── scripts/                # Pipeline scripts and notes
│   └── pipeline_notes.txt
│
├── results/                # Processing results
│   └── results_summary.txt
│
├── figures/                # Visualizations and screenshots
│   └── [screenshots]
│
└── README.md               # Project documentation
```

---

## 🛠️ Tools & Technologies

| Category | Tools |
|:---|:---|
| **Image Processing** | Cryo-EM processing pipelines |
| **Classification** | MSA, HAC, MRA |
| **Reconstruction** | Angular reconstitution, sinogram validation |
| **Visualization** | UCSF Chimera |

---

## ✅ Conclusion

This project demonstrates a **complete cryo-EM SPA pipeline**, highlighting the importance of iterative refinement and classification in achieving high-quality 3D reconstructions.

---

## 🔮 Future Work

- Higher-resolution refinement
- Automated particle picking using **deep learning**
- Integration with **RELION** / **cryoSPARC**
