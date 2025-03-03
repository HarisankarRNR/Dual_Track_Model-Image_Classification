# Dual_Track_Model-Image_Classification

This repository contains code and documentation for the research paper **"A Dual-Track Feature Fusion Model Utilizing Group Shuffle Residual DeformNet and Swin Transformer for the Classification of Grape Leaf Diseases"**. The model combines **global and local feature extraction techniques** to classify grape leaf diseases, achieving **98.6% accuracy** on the PlantVillage dataset.

## About the Paper

This research presents an innovative **Dual-Track Feature Fusion Model** for grape leaf disease classification. The architecture leverages the strengths of both **global and local feature extraction techniques** through two parallel tracks:

### 1. Group Shuffle Residual DeformNet (GSDWR-DC)
This track extracts **local features** by applying:
- Group Shuffle Convolution for enhanced feature representation.
- Residual connections for better gradient flow.
- Deformable Convolutions to capture irregular spatial transformations.

### 2. Swin Transformer
The **Swin Transformer** is used to extract **global contextual information** from the input images, taking advantage of its hierarchical structure and shifted window mechanism.

### 3. Triplet Attention Block
A **Triplet Attention Block** is added to the combined architecture to improve feature refinement by applying **channel, spatial, and cross-dimension attention mechanisms**.

The fusion of both tracks enables the model to effectively classify grape leaf diseases, particularly for datasets like PlantVillage.

## Repository Structure

### 1. [Swin_Transformer-Custom_CNN-triplet.ipynb](Swin_Transformer-Custom_CNN-triplet.ipynb)
This notebook extends the fusion model by integrating **Triplet Attention Block** which gives us the Overall architecture integrating **Swin Transformer, GSDWR-DC, and Triplet Attention Block** achieving **98.6% accuracy**.

### 2. [GSDWR-DC_Custom_CNN.ipynb](GSDWR-DC_Custom_CNN.ipynb)
This notebook implements the **Group Shuffle Residual DeformNet (GSDWR-DC)**, which extracts local features using custom convolutional layers combined with group shuffle and residual connections.

### 3. [Swin_Transformer.ipynb](Swin_Transformer.ipynb)
This notebook implements the **Swin Transformer**, which captures global features using hierarchical multi-head self-attention mechanisms.

### 4. [Swin_Transformer-Custom_CNN.ipynb](Swin_Transformer-Custom_CNN.ipynb)
This notebook combines **Swin Transformer** and **GSDWR-DC** to form the **Dual-Track Feature Fusion Model**, where outputs from both tracks are concatenated and passed through **Triplet Attention Block**.

### 5. [Research Paper - A dual-track feature fusion model.pdf](Research%20Paper%20-%20A%20dual-track%20feature%20fusion%20model%20utilizing%20Group%20Shuffle%20Residual%20DeformNet%20and%20swin%20transformer%20for%20the%20classification%20of%20grape%20leaf%20diseases.pdf)
The full research paper detailing the model architecture, dataset, experiments, and results.

## License
This project is licensed under the **MIT License**.

---
For any queries or collaborations, feel free to reach out via GitHub or email.
