# 🚗🏍️ Car-vs-Bike-Classifier-SVM

> Binary image classification of cars and motorcycles using a Support Vector Machine — built from scratch with NumPy, scikit-learn, and Pillow.

![Python](https://img.shields.io/badge/Python-3.10+-blue?logo=python)
![scikit-learn](https://img.shields.io/badge/scikit--learn-SVM-orange?logo=scikitlearn)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

## 📌 About

A compact machine learning project that classifies grayscale images as either **Car** or **Bike** using a Support Vector Machine (SVM). The pipeline covers image preprocessing, feature scaling, hyperparameter comparison across kernels, and benchmarking against KNN — reaching **83.6% test accuracy**, a 12-point improvement over the KNN baseline.

## ✨ Highlights

- 🖼️ Preprocesses raw images into normalized 64×64 grayscale feature vectors
- ⚙️ Compares 7 SVM configurations (linear & RBF kernels, multiple `C`/`gamma` values)
- 📈 Includes an overfitting analysis (train vs. test accuracy gap per configuration)
- 🆚 Benchmarks SVM against K-Nearest Neighbors (k = 3, 5, 7)
- 📊 Visualizes results with a confusion matrix and classification report

## 📁 Project Structure

```
Car-vs-Bike-Classifier-SVM/
├── SVM.ipynb          # Main notebook: preprocessing, training, evaluation
├── PROJECT.pdf         # Full project report
└── README.md           # This file

```

> 📦 The dataset (`archive.zip`, ~103 MB) is not included in this repo due to GitHub's file size limit. Download it from [Car vs Bike Classification Dataset (Kaggle)](https://www.kaggle.com/datasets/utkarshsaxenadn/car-vs-bike-classification-dataset), extract it, and place the resulting `Car-Bike-Dataset` folder next to `SVM.ipynb`.

## 🗂️ Dataset

This project uses the [Car vs Bike Classification Dataset](https://www.kaggle.com/datasets/utkarshsaxenadn/car-vs-bike-classification-dataset) from Kaggle — 2,000 car images and 2,000 bike images. Download it, extract it, and place the resulting `Car-Bike-Dataset` folder next to `SVM.ipynb`.

## ⚙️ Requirements

```bash
pip install numpy pillow scikit-learn matplotlib seaborn
```

## 🚀 Getting Started

1. Download the dataset from [Kaggle](https://www.kaggle.com/datasets/utkarshsaxenadn/car-vs-bike-classification-dataset) and extract it — this creates the `Car-Bike-Dataset` folder used by the notebook.
2. Open `SVM.ipynb` in VS Code or Jupyter.
3. Run all cells (**Run All**).

## 📊 Results

| Model | Parameters | Test Accuracy |
|-------|-----------|:--------------:|
| **SVM** | RBF kernel, C=10, gamma=0.001 | **83.6%** |
| KNN | k=3 | 71.5% |

> ✅ The SVM model outperformed KNN by ~12 percentage points.

## 🧠 Tech Stack

`Python` · `NumPy` · `Pillow` · `scikit-learn` · `Matplotlib` · `Seaborn`

## 📝 Note

This is a course project for the *Fundamentals of Artificial Intelligence* course, shared here in a lightweight, self-contained form for portfolio purposes.

## 📄 License

This project is released under the MIT License.

## 👩‍💻 Author

**Sepideh Pashayan**
[GitHub](https://github.com/SepidehPashayan)
