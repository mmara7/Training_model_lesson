# Traffic Sign Recognition – Training a CNN for Multi-Class Classification

![Python](https://img.shields.io/badge/python-3.11-blue)
![Jupyter](https://img.shields.io/badge/jupyter-notebook-orange)

This repository addresses the problem of automatically recognizing traffic signs from images.

The goal is to build a model capable of classifying traffic sign images using a Convolutional Neural Network (CNN). This project focuses on the challenges of training a model to accurately recognize multiple classes under varying conditions such as lighting, angles, and image quality.

The demo provides a step-by-step explanation of the technical approach, including data exploration, preprocessing, model simulation, and evaluation.

---

## Project Structure

| Folder | Description |
|--------|-------------|
| `notebooks/` | Jupyter notebooks showing step‑by‑step workflow |
| `docs/` | Written explanations, lessons learned |
| `requirements.txt` | Python dependencies |
| `README.md` | This file |

---
## Problem Statement

Traffic sign recognition is critical for autonomous vehicles and driver-assistance systems.
The main challenge is:

- Training a model that generalizes well across multiple traffic sign classes
- Handling limited data for some classes
- Dealing with variable lighting, angles, and sizes in real-world images

This project demonstrates how to approach these challenges in Python using CNNs, even in a simplified or simulated setting.

---

## Notebooks

| Notebook | Description | Path |
|----------|------------|------|
| 01_data_exploration.ipynb | Explore dataset: visualize images, class distribution, image statistics | [Open](./notebooks/01_data_exploration_and_preprocessing.ipynb) |
| 02_preprocessing.ipynb | Preprocess images: resize, normalize, split train/test, one-hot labels | [Open](./notebooks/02_preprocessing.ipynb) |
| 03_model_training.ipynb | Train CNN (simulated/demo): layer explanation, forward pass, predictions | [Open](./notebooks/03_model_training.ipynb) |
| 04_evaluation.ipynb | Evaluate model: confusion matrix, accuracy, visualizations | [Open](./notebooks/04_evaluation.ipynb) |


---

## Dataset Used

This project is based on the **German Traffic Sign Recognition Benchmark (GTSRB)** dataset — a widely used benchmark dataset for traffic sign classification. It contains **43 classes of German traffic signs** and over **50,000 labeled images** captured under varying conditions (lighting, angles, sizes), making it suitable for developing and testing classification models. ([zenodo.org](https://zenodo.org/doi/10.5281/zenodo.11526387?utm_source=chatgpt.com))

Dataset link: https://zenodo.org/records/13741936

> Note: The dataset is not included in this repository due to size — instead, notebook examples use small simulated data for demonstration purposes.

---

## Tech Stack

This walkthrough uses the following Python libraries:

- `numpy` – numerical operations  
- `tensorflow` / `keras` – building and training CNNs  
- `matplotlib` – plotting and visualization
- `opencv-python` – image preprocessing

---

## Model Architecture

| Layer (type)        | Output Shape | Param # |
|--------------------|-------------|---------|
| Conv2D              | (30, 30, 16) | 448     |
| MaxPooling2D        | (15, 15, 16) | 0       |
| Flatten             | (3600,)      | 0       |
| Dense (Fully Connected) | (128,)    | 460928  |
| Dense (Output)      | (43,)        | 5547    |

> Tip: This architecture is simplified for demo purposes. Full CNN training would involve multiple Conv/Pool layers and proper regularization.

---

##  How to Run

1. Clone the repository:

```bash
git clone https://github.com/mmara7/Training_model_lesson.git
```
---

2. Install dependencies:

```bash
pip install -r requirements.txt
```
---

3. Open Jupyter Notebook:

```bash
jupyter notebook
```
---

4. Open the notebook notebooks/01_data_exploration.ipynb and follow the instructions.

What You Will Learn
- How to explore and visualize traffic sign data

- How to preprocess images for CNN input

- How to build, train, and troubleshoot a simple CNN model

- Common issues in training and how to address them
