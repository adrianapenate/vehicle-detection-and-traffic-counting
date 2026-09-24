# Vehicle Detection in Traffic Videos

Computer vision project focused on detecting and counting vehicles in traffic videos using image processing techniques and OpenCV.

## 🚗 Project Overview

The project analyzes vehicle traffic through background subtraction, contour detection, regions of interest (ROI), and lane-based counting.

The initial approach presented issues such as:

- Shadows being detected as part of vehicles
- Multiple nearby vehicles being detected as a single object
- Repeated vehicle counting

The improved solution addresses these limitations using `BackgroundSubtractorMOG2`, shadow detection, morphological filters, specific ROIs, and independent lane counters. fileciteturn1file0L27-L38

## 🔎 Methodology

The main detection pipeline includes:

- Video frame reading with OpenCV
- Background subtraction with `BackgroundSubtractorMOG2`
- Shadow detection
- Morphological opening and closing
- Contour detection
- Definition of regions of interest (ROI) for each lane
- Independent vehicle counters
- Cooldown mechanism to prevent duplicate counts
- Real-time visualization of ROIs and counters fileciteturn1file1L69-L80

## 📊 Results

The improved approach reduced false positives caused by shadows, improved the detection of nearby vehicles, reduced image noise, and enabled more reliable lane-by-lane counting, including in dense traffic scenarios. fileciteturn1file1L81-L95

## 📁 Project Structure

```text
├── Deteccion_de_vehiculos.ipynb
├── Opcional 1.ipynb
├── Opcional 2.ipynb
├── Opcional 3.ipynb
├── Opcional 4.ipynb
└── Memoria.pdf
```

The main notebook processes `trafico.mp4`. The optional notebooks contain alternative configurations for different traffic videos (`trafico1.mp4`–`trafico4.mp4`) and different ROI/lane setups.

## ⚙️ Requirements

The project was developed in Python and uses:

- Python 3
- OpenCV (`cv2`)
- NumPy

## ▶️ How to Run

Open `Deteccion_de_vehiculos.ipynb` in Jupyter Notebook, JupyterLab, or Google Colab.

Place the corresponding traffic video files in the same directory as the notebook and run the cells sequentially.

## 📄 Documentation

`Memoria.pdf` contains the project documentation, including the initial approach, identified limitations, improved solution, workflow, results, and conclusions.

## 🎯 Objective

The project demonstrates how image processing techniques can be combined to build a practical vehicle detection and counting system for traffic videos. 

## 👤 Authors

Adriana Peñate Sosa → [@adrianapenate](https://github.com/adrianapenate)
Sofía Travieso García → [@sofiatravieso](https://github.com/sofiatravieso)

