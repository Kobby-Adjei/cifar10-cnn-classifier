# cifar10-cnn-classifier
Here you go — run this in your terminal:



Experimenting with CNN architectures to classify images from the CIFAR-10 dataset using TensorFlow and Keras.

## Overview

The CIFAR-10 dataset consists of 60,000 32x32 color images across 10 classes (airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck). This project experiments with 3 different CNN architectures to find the best balance between accuracy and training efficiency.

## Architectures

| | CNN 1 (Simple) | CNN 2 (Medium) | CNN 3 (Deep) |
|---|---|---|---|
| Conv Layers | 2 | 3 | 4 |
| Kernels | 32/64 | 64/128/128 | 64/128/128/256 |
| Dense Layers | 1 (64 neurons) | 1 (128 neurons) | 2 (256+128 neurons) |
| Training Time | 715s | 1988s | 2422s |
| Test Accuracy | 68.07% | 71.02% | 71.89% |

## Key Findings

- CNN 2 offers the best balance between accuracy and compute efficiency
- Increasing model complexity improved accuracy but with diminishing returns
- All models showed overfitting that worsened with complexity
- CNN 3 took 434 more seconds than CNN 2 for less than 1% accuracy gain

## Tech Stack

- Python 3
- TensorFlow / Keras
- Google Colab (T4 GPU)

## How to Run

Install dependencies:
```
pip install tensorflow
```

Run any of the three CNN scripts:
```
python cnn1_simple.py
python cnn2_medium.py
python cnn3_deep.py
```

## Project Structure

```
cifar10-cnn-classifier/
├── cnn1_simple.py
├── cnn2_medium.py
├── cnn3_deep.py
└── README.md
```

## Course

COSC 480/592: Embedded AI -- Eastern Michigan University
EOF
```

Then push it:
```bash
git add .
git commit -m "Add README"
git push https://YOUR_TOKEN@github.com/Kobby-Adjei/cifar10-cnn-classifier.git master
```
