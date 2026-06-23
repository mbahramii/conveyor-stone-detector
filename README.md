# 🚧 Conveyor Stone Detector

A real-time computer vision system for detecting stones on a conveyor belt using OpenCV.  
This project uses classical image processing techniques (no deep learning) to detect and highlight objects based on shape and area.

---

## 🎯 Project Goal

The goal of this project is to detect stones in a conveyor belt video stream using traditional computer vision techniques, without using neural networks or deep learning models.

---

## 🧠 How It Works (Pipeline)

```text
Video Frame
↓
Region of Interest (ROI)
↓
Grayscale Conversion
↓
CLAHE (Contrast Enhancement)
↓
Gaussian Blur (Noise Reduction)
↓
Adaptive Thresholding
↓
Morphological Operations
↓
Contour Detection
↓
Object Filtering (Area-based)
↓
Stone Detection Result
```

---

## ⚙️ Features

- Real-time video processing
- ROI-based detection (focus only on conveyor area)
- Adaptive threshold segmentation
- Noise removal using morphology
- Object area & size estimation (in pixels)
- Bounding box visualization
- Stone / No-Stone classification

---

## 🛠️ Technologies Used

- Python
- OpenCV
- NumPy

---

## 📁 Project Structure

```text
Stone.ipynb → Main notebook (Colab)
input.mp4 → Input video
output_area.mp4 → Processed output video
README.md → Project documentation
```

---

## 🎥 Demo

You can view the output video here:

 [Download / View Video](output_area.mp4)

---

## 📊 Output Description

For each detected object:

- Bounding box is drawn
- Area is calculated in pixels
- Width and height are estimated
- Status is displayed:
  - STONE
  - NO STONE

---

## 🚀 How to Run

1. Open `Stone.ipynb` in Google Colab  
2. Upload input video (`input.mp4`)  
3. Run all cells  
4. Get output video (`output_area.mp4`)

---

## 📌 Notes

- This project uses classical computer vision only
- No deep learning (YOLO, CNN, etc.)
- Performance depends on lighting and camera quality
- ROI is manually defined for conveyor belt region

---

## 👨‍💻 Author

- Name: Mohammad Bahramii
- GitHub: https://github.com/mbahramii  
- Project: Conveyor Stone Detector  
---

## ⭐ Future Improvements

- Replace contour-based detection with YOLO or deep learning
- Add real-world calibration (cm instead of pixels)
- Add multi-object tracking
- Improve robustness under different lighting conditions
```
