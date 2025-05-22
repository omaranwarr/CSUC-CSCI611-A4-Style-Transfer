# Style Transfer with Deep Neural Networks

This project implements neural style transfer using a pre-trained VGG19 convolutional neural network. The goal is to generate a new image that preserves the **content** of one image while adopting the **style** of another, based on the work of *Gatys et al.*

---

## 📁 Project Structure

```
├── style_transfer.ipynb                # Final completed notebook
├── starry_stylized_output.png          # Final stylized image
├── blue_lake.png                       # style image
├── starry_night_van_gogh.png           # style image
└── README.md                           # This file
```

---

## 🚀 Getting Started

### 1. Clone this repository or download the files
```bash
git clone https://github.com/yourusername/CSUC-CSCI611-A4-Style-Transfer
cd style-transfer-pytorch
```

### 2. Install required packages
```bash
pip install torch torchvision matplotlib pillow requests
```

### 3. Run the notebook
Open `style_transfer.ipynb` in Jupyter Notebook or VS Code and run all cells.

---

## ⚙️ Features

- Uses a pre-trained **VGG19** model for feature extraction
- Computes **content loss** and **style loss** using Gram matrices
- Optimizes a target image to match content and style features
- Adjustable hyperparameters for fine-tuning output
- Final image is saved to disk

---

## 🎯 Hyperparameters

You can experiment with the following:

| Parameter        | Default | Description                            |
|------------------|---------|----------------------------------------|
| `content_weight` | `1`     | Emphasizes content structure           |
| `style_weight`   | `5e6`   | Emphasizes style textures              |
| `steps`          | `10000` | Number of training iterations          |
| `lr`             | `0.003` | Learning rate for Adam optimizer       |
| `style_layers`   | `conv1_1`, `conv3_1` | Layers used for style features |

---

## 🖼️ Output

Final stylized image is saved as:

```
starry_stylized_output.png
```

---


