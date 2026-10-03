
---

# README — Experiment 7

```markdown
# Experiment 7 — K-Nearest Neighbors Classification

## Objective

To implement the **K-Nearest Neighbors (KNN)** classification algorithm using the **Fashion-MNIST dataset** and study the effect of different values of **K** on classification accuracy and inference time.

---

## Dataset

The experiment uses the Fashion-MNIST dataset containing grayscale images of clothing and footwear.

### Original Dataset

- Training images: 60,000
- Testing images: 10,000
- Image size: 28 × 28 pixels

For this experiment, a stratified subset was selected:

- Training images: **10,000**
- Testing images: **2,000**

The notebook records the original dataset shapes as `(60000, 28, 28)` and `(10000, 28, 28)`. :contentReference[oaicite:5]{index=5}

---

## Classes

The dataset contains 10 classes:

| Label | Class |
|---:|---|
| 0 | T-shirt/top |
| 1 | Trouser |
| 2 | Pullover |
| 3 | Dress |
| 4 | Coat |
| 5 | Sandal |
| 6 | Shirt |
| 7 | Sneaker |
| 8 | Bag |
| 9 | Ankle boot |

---

## Data Preprocessing

The following preprocessing steps were performed:

1. Stratified sampling of the dataset
2. Selection of 10,000 training images
3. Selection of 2,000 testing images
4. Flattening of 28 × 28 images
5. Conversion into 784-dimensional feature vectors
6. Normalization of pixel values by dividing by 255

The resulting processed shapes are:

```text
Training: (10000, 784)
Testing : (2000, 784)
