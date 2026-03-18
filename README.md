# 🔬 Cryo-EM Single Particle Analysis (SPA) Pipeline

## 📌 Project Overview

This project demonstrates a full **Single Particle Analysis (SPA)** workflow in cryo-electron microscopy, from raw particle images to 3D reconstruction.

---

## 🎯 Objectives

* Process particle images from cryo-EM data
* Perform alignment and classification
* Generate and refine 3D structures
* Validate reconstruction quality

---

## ⚙️ Workflow

### 1. Sample Preparation

* Purification and vitrification of biological samples
* Preservation of native structure in vitreous ice

---

### 2. Data Acquisition

* Captured thousands of particle projections using TEM
* Controlled parameters: defocus, contrast, electron dose

---

### 3. Particle Picking & Extraction

* Identified particles using computational methods
* Extracted particles into boxed images
* Applied masking to focus on relevant regions

---

### 4. Alignment & Classification

* Aligned particles to a common reference
* Performed:

  * 2D classification
  * 3D classification
* Selected high-quality classes

---

### 5. 3D Reconstruction

* Generated initial 3D model (ab initio)
* Refined using iterative alignment

---

### 6. Model Refinement

* Improved structure using:

  * Symmetry constraints
  * Real-space refinement
* Validated results with reprojections

---

## 📊 Key Processing Steps

* Bandpass filtering to remove noise
* Particle centering using alignment algorithms
* Multivariate Statistical Analysis (MSA)
* Hierarchical classification (HAC)
* Angular reconstitution (Euler angles)
* Sinogram validation
* Multi-reference alignment (MRA)

---

## 📈 Results

* Successfully reconstructed 3D models:

  * `3d_0-1`
  * `3d_0-2`
* Improved alignment and consistency with additional views
* Final models visualized in Chimera

---

## 🛠️ Tools & Technologies

* Cryo-EM processing tools
* Chimera (visualization)
* Image processing pipelines

---

## 📂 Project Structure

```
cryo-em-project/
│
├── README.md
├── report/
│   └── cryo_em_report.pdf
├── scripts/
│   └── pipeline_notes.txt
├── results/
│   └── results_summary.txt
├── figures/
│   └──  screenshots 
```

## ✅ Conclusion

This project demonstrates a complete cryo-EM SPA pipeline, highlighting the importance of iterative refinement and classification in achieving high-quality 3D reconstructions.

---

## 📌 Future Work

* Higher-resolution refinement
* Automated particle picking (deep learning)
* Integration with RELION / cryoSPARC
