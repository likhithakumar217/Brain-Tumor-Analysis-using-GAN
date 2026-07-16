# 🧠 Fusion of MRI and CT Images Using GAN for Brain Tumor Analysis

## 📌 Project Overview

This project presents a deep learning-based medical image fusion framework that combines Magnetic Resonance Imaging (MRI) and Computed Tomography (CT) images using a Generative Adversarial Network (GAN). The proposed model preserves the complementary information from both modalities, producing a single fused image with improved structural and anatomical details to assist in brain tumor analysis.

The model utilizes dual encoders, residual learning, hybrid activation functions, and PixelShuffle-based upsampling to generate high-quality fused images while reducing blur and preserving fine details.

---

## 🎯 Objectives

- Fuse MRI and CT brain images into a single informative image.
- Preserve soft tissue information from MRI.
- Preserve bone and structural information from CT.
- Improve image quality using deep learning.
- Reduce blurring artifacts.
- Generate high-resolution fused medical images.

---

## 🏗 Proposed Architecture

The proposed Generator consists of:

- Dual Encoder Network
- Residual Learning Blocks
- Feature Concatenation
- PixelShuffle Decoder
- GAN-based Image Generation

### Encoder

- Convolution Layers
- Instance Normalization
- PReLU (Shallow Layers)
- Mish Activation (Deep Layers)

### Residual Blocks

- Convolution
- InstanceNorm
- Mish
- Swish
- Skip Connections

### Decoder

- Convolution
- PixelShuffle Upsampling
- InstanceNorm
- Mish Activation

### Output Layer

- Convolution
- Tanh Activation

---

## 📂 Dataset

The project uses paired MRI and CT brain images.

Folder Structure

dataset/

├── MRI/

│ ├── img1.png

│ ├── img2.png

│ └── ...

├── CT/

│ ├── img1.png

│ ├── img2.png

│ └── ...

---

## 🛠 Technologies Used

- Python
- PyTorch
- OpenCV
- NumPy
- Matplotlib
- Google Colab

---

## 📦 Python Libraries

```bash
pip install torch torchvision
pip install opencv-python
pip install matplotlib
pip install numpy
pip install scikit-image