# TreeSense  
**Estimating carbon storage of individual trees using UAV imagery and human-in-the-loop machine learning**

---

### Problem

Tree-level carbon estimation is vital but traditionally slow, costly, and limited in scale. UAV imagery offers scalability, but extracting features like DBH or species is hard from RGB images alone. Automated methods often fail in dense forests, and existing tools lack intuitive 3D interaction.

---

### Solution Overview

TreeSense bridges the gap between UAV data and reliable carbon estimates. It automates 3D forest modeling and tree feature extraction, lets users provide ground-truth data to train predictive models, and offers tools to refine results manually. Immersive 3D visualization enables better understanding and validation.

#### Features

- **3D Forest Modeling** – Builds DSM, DTM, and CHM from UAV RGB images  
- **Tree Segmentation** – Groups and extracts tree-level metrics (height, canopy size, etc.)  
- **User-Trained Prediction** – Estimate DBH/species using user-supplied data + regression  
- **Interactive Corrections** – Manually adjust tree groupings (merge, split, add, delete)  
- **Immersive Visualization** – Explore results in 3D using Gaussian Splatting (3DGS)  
- **Carbon Estimation** – Compute biomass and carbon per tree

---
