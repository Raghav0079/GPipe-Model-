# GPipe-Model-
# 🚀 GPipe + AmoebaNet on CIFAR-10  

This project demonstrates **scalable neural network training** using **GPipe pipeline parallelism** with **AmoebaNet-Small** and **Transformer-based** architectures on the **CIFAR-10 dataset**.  

The implementation is lightweight enough to run on **Google Colab Free/Pro**, but also supports **W&B tracking**, **Gradio UI**, and **Hugging Face Hub deployment** for real-world usage.  

---

## 📖 Table of Contents
- [About GPipe](#about-gpipe)  
- [About AmoebaNet](#about-amoebanet)  
- [Project Features](#project-features)  
- [Installation](#installation)  
- [Project Structure](#project-structure)  
- [Training](#training)  
- [Experiment Tracking (Weights & Biases)](#experiment-tracking-weights--biases)  
- [Gradio UI Demo](#gradio-ui-demo)  
- [Deployment on Hugging Face](#deployment-on-hugging-face)  
- [Results](#results)  
- [Next Steps](#next-steps)  
- [Author](#author)  

---

## 📌 About GPipe  

**GPipe** is a scalable **pipeline parallelism** framework for training large neural networks efficiently.  

- Splits a deep model into **stages** across multiple devices.  
- Uses **micro-batching** to keep all devices busy (minimizing idle time).  
- Allows training models with **billions of parameters** without running out of memory.  

📄 Paper: *[GPipe: Efficient Training of Giant Neural Networks using Pipeline Parallelism](https://arxiv.org/abs/1811.06965)*  

---

## 📌 About AmoebaNet  

**AmoebaNet** is a **Neural Architecture Search (NAS)**-designed model from Google Brain. It automatically learns efficient CNN architectures by evolutionary search.  

In this project, we use **AmoebaNet-Small**, which is lightweight enough for **CIFAR-10 classification** on Colab.  

📄 Paper: *[Regularized Evolution for Image Classifier Architecture Search](https://arxiv.org/abs/1802.01548)*  

---

## ✨ Project Features  

- ✅ GPipe implementation with PyTorch  
- ✅ AmoebaNet-Small & Transformer on CIFAR-10  
- ✅ Training on **Colab Free (T4 GPU)**  
- ✅ Automatic checkpoint saving & resume  
- ✅ W&B experiment logging  
- ✅ Gradio-powered interactive demo  
- ✅ Hugging Face model hosting & Space deployment  

---


## Colab Notebook 

https://colab.research.google.com/drive/1TRTdU60KI_2SZmL8dHcwUSaf2o_2-T96?usp=drive_link


## ⚙️ Installation  

Clone the repo:  
```bash
git clone https://github.com/your-username/gpipe-amoebanet.git
cd gpipe-amoebanet

