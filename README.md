# Iris Biometric Recognition System 👁️🔐

An end-to-end **Iris Biometric Recognition System** built using **Python and OpenCV**, implementing classical computer vision algorithms for accurate iris localization, feature extraction, and identity matching.

---

## 📌 Overview

Iris recognition is one of the most reliable biometric authentication techniques due to the **uniqueness, stability, and complexity** of iris texture patterns.  
This project implements a **complete iris recognition pipeline** without deep learning, focusing on **interpretable and efficient classical methods**.

---

## 🧠 Key Features

- Robust preprocessing to handle noise and lighting variations  
- Accurate iris localization using **Circular Hough Transform**  
- Iris normalization using the **Rubber Sheet Model**  
- Texture-based feature extraction using **2D Gabor Wavelets**  
- Fast and reliable matching using **Hamming Distance**  

---

## 🔁 System Pipeline

Eye Image
→ Preprocessing
→ Iris Localization & Segmentation
→ Normalization
→ Feature Extraction
→ Matching & Decision

---

## 🛠️ Technologies Used

- **Python**
- **OpenCV**
- **NumPy**
- **Matplotlib** (for visualization)

---

## ⚙️ Methodology

### 1️⃣ Image Preprocessing
- Grayscale conversion  
- Median filtering to remove salt-and-pepper noise  
- Gamma correction to improve brightness and contrast  

**Purpose:** Enhance iris boundaries and reduce noise before segmentation.

---

### 2️⃣ Iris Localization & Segmentation
- Iris and pupil boundaries are detected using **Circular Hough Transform**
- Exploits the circular nature of the iris and pupil

**Purpose:** Accurately isolate the iris region from the eye image.

---

### 3️⃣ Iris Normalization
- The segmented iris is transformed into a fixed-size rectangular representation using the **Rubber Sheet Model**
- Converts polar coordinates into Cartesian coordinates

**Purpose:** Handle scale and pupil dilation variations.

---

### 4️⃣ Feature Extraction
- **2D Gabor Wavelets** are applied to the normalized iris image
- Only **phase information** is used to generate a binary iris code

**Purpose:** Extract unique, illumination-invariant texture features.

---

### 5️⃣ Matching
- Iris codes are compared using **Hamming Distance**
- A predefined threshold determines **Match / No Match**

**Purpose:** Measure similarity between two iris patterns efficiently.

---

## 📊 Matching Criteria

- **Hamming Distance ≤ 0.38** → Match  
- **Hamming Distance > 0.38** → No Match  

This threshold balances false acceptance and false rejection rates.

---

## 🎯 Results

- Reliable iris localization under varying lighting conditions  
- Robust feature extraction insensitive to illumination changes  
- Efficient and accurate identity verification  

---

## 🚀 Future Improvements

- Handle heavy occlusions (eyelids/eyelashes) more robustly  
- Integrate deep learning–based segmentation for real-world datasets  
- Optimize pipeline for real-time authentication systems  


#Thankyou
