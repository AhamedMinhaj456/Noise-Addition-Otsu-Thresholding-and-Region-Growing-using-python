# EC7212 – Computer Vision and Image Processing - Take Home 02

This repository contains Python implementations of:

1. **Otsu's Thresholding** on a noisy image.
2. **Region Growing Segmentation** using seed points and color similarity.

---

## 📂 Project Structure

```
├── original_image.png               # Input image (user-provided)
├── takeHome2.ipynb                  # Main script with all operations
├── README.md                        # Readme file
└── EC7212_4076_Assignment_2.pdf # This file for description
```

---

## 📌 Requirements

Make sure the following Python libraries are installed:

```bash
pip install numpy opencv-python matplotlib
```

---

## ▶️ How to Run

1. **Place your input image** in the project folder and name it `input.png`.
2. **Run the script** in a terminal or IDE:

```bash
python takeHome2.ipynb
```

3. The script will:
   - Load and display the original image.
   - Add Gaussian noise.
   - Apply Otsu’s thresholding.
   - Show the binary segmentation result.
   - Perform region-growing from seed points.
   - Visualize the region mask and overlay.

---

## 🧪 Features Implemented

### ✅ Part 1: Otsu’s Thresholding
- Adds Gaussian noise to RGB image.
- Converts to grayscale.
- Computes Otsu threshold manually.
- Displays segmented binary image.

### ✅ Part 2: Region Growing
- Allows manual seed point definition.
- Expands region based on color similarity.
- Generates binary mask and overlay output.

---

## 📸 Sample Output

| Step                      | Output Description              |
|--------------------------|---------------------------------|
| Original Image           | Loaded from `original_image.png`         |
| Noisy Image              | After Gaussian noise addition   |
| Histogram                | Grayscale histogram             |
| Binary Image             | Otsu threshold result           |
| Region-Grown Mask        | From seed points                |
| Overlay Segmentation     | Red-highlighted region on image |

---

## 📬 Notes
- You can change the seed points or tolerance value in the script for different results.
- Works with any 3-channel color image.
