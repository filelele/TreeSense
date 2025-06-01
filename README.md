# TreeSense
Leveraging Unarmed Aerial Vehicle images to calculate carbon storage of trees
---
### 1. Problem Statement

Estimating forest biomass and carbon at the individual tree level is critical for sustainable forestry, ecological research, and climate change mitigation. Traditional field-based surveys are slow, labor-intensive, and costly, making them impractical for large-scale or repeated assessments.

UAV imagery presents a promising alternative due to its high spatial resolution and scalability. Yet, significant challenges remain. Extracting key attributes like diameter at breast height (DBH) or tree species is difficult using RGB images alone. Automated canopy segmentation often struggles in dense or overlapping forest conditions, leading to inaccurate tree delineation. Additionally, many existing tools lack intuitive ways for users to interact with or validate 3D forest data.

These limitations create a gap between raw drone data and reliable, actionable insights for forest carbon estimation. TreeSense aims to bridge this gap with a hybrid, human-in-the-loop platform that combines automated processing, user input, and immersive 3D visualization.

---
### 2. Solution Overview

TreeSense provides a practical, hybrid approach to tree-level forest carbon estimation using UAV RGB imagery. It automates 3D forest modeling and the extraction of key tree features. For unobtainable directly data like DBH or species, it uniquely combines user-provided ground truth with machine learning to train custom prediction models. The platform also allows manual refinement of tree groupings for accuracy, all presented with immersive 3D visualization. TreeSense blends automation and human expertise for more accurate and usable drone-based forest assessments.

### Features

- Automated 3D Forest Modeling: Transforms UAV images into detailed 3D representations of forest plots.
- Automatic Tree Grouping & Feature Extraction: Identifies and segments individual tree canopies, then extracts parameters like height and canopy dimensions.
- Immersive 3D Visualization: Utilizes 3D Gaussian Splatting (3DGS) for high-quality, intuitive exploration of the forest.
- Human-in-the-Loop Machine Learning:
  - User-Trained Prediction Models: Allows users to input manual data (e.g., DBH) for a subset of trees to train a simple regression model, predicting these values for others.
  - Reusable Model Presets: Save and load trained prediction models for future use.
- Interactive Group Correction: Provides tools to manually refine and correct automated tree canopy groupings (merge, split, add, delete).

==> Tree-Level Carbon Estimation: Calculates biomass and carbon for individual trees using combined automated and user-refined data.



