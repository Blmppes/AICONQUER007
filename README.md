# Breast Cancer Risk Prediction

A web-based application that predicts breast cancer risk using Logistic Regression implemented from scratch. The model performs client-side inference directly in the browser without requiring a backend server.

This project is part of **AI Conquer** program, an initiative by **AI Vietnam**.

## Overview

This project implements a machine learning solution for breast cancer classification based on tumor characteristics. The model analyzes 30 features extracted from digitized images of fine needle aspirate (FNA) of breast masses to predict whether a tumor is **benign** or **malignant**.

## Features

- **Client-side inference**: All predictions run directly in the browser using JavaScript
- **Logistic Regression from scratch**: Custom implementation without external ML libraries
- **Real-time predictions**: Instant results upon form submission
- **Interactive UI**: Tooltips provide explanations for each input feature
- **Responsive design**: Modern gradient-based interface

## Input Features

The model accepts 30 features grouped into three categories:

### Mean Features
- Radius, Texture, Perimeter, Area
- Smoothness, Compactness, Concavity
- Concave Points, Symmetry, Fractal Dimension

### Error Features
- Standard error measurements for all 10 base features

### Worst Features
- Largest values (mean of three largest) for all 10 base features

## Project Structure

```
AICONQUER007/
├── index.html          # Main application interface
├── script.js           # Logistic regression model and inference logic
├── style.css           # Application styling
├── doc/
│   └── ProjectSlide.pptx   # Project presentation
└── project_pic/        # Project images
    └── pic1-12.jpg
```

## How It Works

1. **Feature Input**: User enters 30 tumor measurements
2. **Standardization**: Input values are normalized using pre-computed mean and standard deviation
3. **Linear Combination**: Standardized features are combined with trained weights
4. **Sigmoid Activation**: Output is transformed to probability using the sigmoid function
5. **Classification**: Probability >= 0.5 indicates malignant, otherwise benign

## Usage

1. Open `index.html` in a web browser
2. Enter the tumor feature measurements in the form fields
3. Click "Predict Risk" to get the prediction
4. View the result showing classification and probability

## Technologies

- HTML5
- CSS3
- Vanilla JavaScript

## Dataset

The model was trained on the Wisconsin Breast Cancer Dataset, which contains measurements computed from digitized images of fine needle aspirates of breast masses.

## Links

- **Web Demo**: https://blmppes.github.io/AICONQUER007/
- **Project Slide**: https://github.com/Blmppes/AICONQUER007/blob/main/doc/ProjectSlide.pptx
- **Project Blog (Vietnamese)**: https://aioconquer.aivietnam.edu.vn/posts/logistic-regression-from-scratch-hieu-gradient-thong-qua-ma-tran
- **Project Blog (English)**: https://aioconquer.aivietnam.edu.vn/posts/logistic-regression-from-the-start-understanding-the-gradient-through-matrices

## Team Members

- [Nguyễn An Phương Linh](https://github.com/Freya-Ng)
- Đỗ Cẩm Nhung
- Nguyễn Hoài Nam
- Vũ Minh Hiếu
- [Đỗ Trung Hiếu](https://github.com/Blmppes)

---

*This project was developed for educational purposes as part of the AI Conquer program by AI Vietnam to demonstrate machine learning concepts and web-based model deployment.*
