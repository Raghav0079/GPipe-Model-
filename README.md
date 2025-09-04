# 🚀 GPipe + AmoebaNet on CIFAR-10  

This project demonstrates **scalable neural network training** using **GPipe pipeline parallelism** with **AmoebaNet-Small** and **Transformer-based** architectures on the **CIFAR-10 dataset**.  

The implementation is lightweight enough to run on **Google Colab Free/Pro**, but also supports **W&B tracking**, **Gradio UI**, and **Hugging Face Hub deployment** for real-world usage.  

---


## � Overview

This project demonstrates **GPipe pipeline parallelism** with **AmoebaNet-Small** and **Transformer** models on the **CIFAR-10 dataset**. It is designed for scalable training, experiment tracking, and easy deployment.

---


## 🗂️ Table of Contents

- [Features](#features)
- [Project Structure](#project-structure)
- [Setup & Installation](#setup--installation)
- [Colab Notebook](#colab-notebook)
- [Usage](#usage)
- [Experiment Tracking](#experiment-tracking)
- [Gradio Demo](#gradio-demo)
- [Deployment](#deployment)
- [Results](#results)
- [Next Steps](#next-steps)
- [Author](#author)

---

## ✨ Features

- GPipe pipeline parallelism (PyTorch)
- AmoebaNet-Small & Transformer models
- CIFAR-10 classification
- Colab/Local training support

## 📓 Colab Notebook

[Open in Colab](https://colab.research.google.com/drive/1TRTdU60KI_2SZmL8dHcwUSaf2o_2-T96?usp=drive_link)

---

## 🚦 Usage

Train a model:

```bash
python gpipe_amoebanet.py --config config.yaml
```

Or use the [Colab Notebook](https://colab.research.google.com/drive/1TRTdU60KI_2SZmL8dHcwUSaf2o_2-T96?usp=drive_link) for step-by-step training.

---

## 📚 About GPipe

**GPipe** is a scalable pipeline parallelism framework for training large neural networks efficiently. It splits a deep model into stages across multiple devices and uses micro-batching to keep all devices busy, minimizing idle time. This enables training models with billions of parameters without running out of memory.

**Reference:**
> Huang et al., "GPipe: Efficient Training of Giant Neural Networks using Pipeline Parallelism" ([arXiv:1811.06965](https://arxiv.org/abs/1811.06965))

---

## 🧬 About AmoebaNet

**AmoebaNet** is a Neural Architecture Search (NAS)-designed model from Google Brain. It automatically learns efficient CNN architectures by evolutionary search. In this project, we use AmoebaNet-Small, which is lightweight enough for CIFAR-10 classification on Colab.

**Reference:**
> Real et al., "Regularized Evolution for Image Classifier Architecture Search" ([arXiv:1802.01548](https://arxiv.org/abs/1802.01548))

---

## � Experiment Tracking

This project integrates [Weights & Biases](https://wandb.ai/) for:
- Logging training/validation metrics
- Visualizing loss, accuracy, and hyperparameters
- Comparing multiple runs and configurations

**How to use:**
1. Login with `wandb login`
2. Training logs will be automatically synced
3. View results on your W&B dashboard

---

## 🎛️ Gradio Demo

Run the interactive demo locally:

```bash
python gradio_app.py
```

**Features:**
- Upload an image and get CIFAR-10 class prediction
- Visualize model confidence and output
- Try both AmoebaNet and Transformer models

---

## � Deployment

**Hugging Face Hub:**
- Share trained models with the community
- Version control and easy download

**Gradio Spaces:**
- Deploy interactive demos for public use

---


It is ideal for students, researchers, and ML engineers interested in distributed training, NAS, and practical deployment workflows.

---


## 📈 Results

| Model            | Accuracy | Hardware      |
|------------------|----------|--------------|
| AmoebaNet-Small  | 94%      | Colab T4 GPU |
| Transformer      | 92%      | Colab T4 GPU |

---

## 🔮 Next Steps

- Support for larger datasets (ImageNet)
- More NAS architectures
- Multi-GPU optimization
- Enhanced Gradio UI features

---

## 👤 Author

**Raghav0079**  
GitHub: [Raghav0079](https://github.com/Raghav0079)

=======