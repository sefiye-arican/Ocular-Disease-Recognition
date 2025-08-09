This project was carried out as an undergraduate capstone project in collaboration with [@Ahmet Selçuk KÜREN](https://github.com/as-krn).

---

# 🩺 Multi-Disease Detection from Fundus Images Using an Attention-Enhanced Deep Learning Model

This project is an **attention-enhanced deep learning-based** diagnostic system that enables the **simultaneous detection of multiple eye diseases from fundus images**.\
In this study, **CLAHE** and **ESRGAN** techniques were used to improve image quality, and **Channel & Spatial Attention** mechanisms were integrated into transfer learning models to enhance performance.

---

## 📌 Objective

- Automatic detection of **glaucoma, diabetic retinopathy, cataract, age-related macular degeneration (AMD), hypertension, myopia, other, and normal** categories from fundus images.
- Enhancing the visibility of pathological findings through image preprocessing techniques.
- Improving the detection of small and localized abnormalities by integrating **attention mechanisms** into deep learning architectures.

---

## 📂 Dataset

- **ODIR-5K (Ocular Disease Intelligent Recognition)** dataset was used.
- **10,000 fundus images** from 5,000 patients (right/left eye).
- Classes:
  - `Normal`
  - `Diabetic`
  - `Glaucoma`
  - `Cataract`
  - `Age-related Macular Degeneration (AMD)`
  - `Hypertension`
  - `Myopia`
  - `Other`

---

## 🛠 Methods and Architectures Used

1. **Preprocessing**
   - **CLAHE**: Increasing local contrast
   - **Cropping**: Isolating the fundus region
   - **Color Conversions**: BGR → LAB → BGR → RGB

2. **Super-Resolution Enhancement**
   - **ESRGAN**: Converting low-resolution fundus images into high-resolution ones

3. **Attention Mechanisms**
   - **Channel Attention (CA)**
   - **Spatial Attention (SA)**

4. **Deep Learning Models (Transfer Learning)**
   - VGG16
   - MobileNetV2
   - EfficientNetB0
   - ResNet50

---

## 📊 Results

- The integration of **ESRGAN + Attention** improved accuracy and F1 scores across all models.
- EfficientNetB0 achieved the highest performance when preprocessing and attention mechanisms were applied.
- Class-based evaluations showed improvement in detecting rare diseases.

---

## 📈 Training Environment

- Python 3.9+
- TensorFlow / Keras
- NumPy, Pandas, Matplotlib
- OpenCV
- PyTorch (for ESRGAN)

---
