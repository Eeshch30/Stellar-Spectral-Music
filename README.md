# 🌌 Stellar Spectral Music
### Sonifying the Hertzsprung–Russell Diagram using Machine Learning and Astronomy

Stellar Spectral Music is a data science and interactive sonification project that transforms stellar properties into music.

Using real astronomical data, this project analyzes stars, classifies stellar populations using machine learning, detects unusual stars through anomaly detection, and converts physical stellar properties into musical motifs and sound.

The goal is to create an experience where users can **see, explore, and hear the differences between stars**.

---

## 🎯 Project Goals

This project combines:

- Astronomy
- Data Science
- Machine Learning
- Audio Generation
- Interactive Visualization

Users can:

⭐ Explore an interactive HR diagram  
🎵 Hear stars as generated musical phrases  
🔮 Predict stellar class from physical properties  
⚠ Discover anomalous or unusual stars  
📊 Visualize relationships between stellar features  

---

## 🌌 Dataset

Primary dataset:

- Gaia DR3 stellar catalogue

Features used:

- Effective Temperature (`teff_gspphot`)
- Apparent Magnitude (`phot_g_mean_mag`)
- Color Index (`bp_rp`)
- Parallax

Derived features:

- Absolute Magnitude
- Log Temperature
- Log Luminosity
- Interaction Features

---

## 🧹 Data Pipeline

### 1. Data Collection
Acquire stellar observations from Gaia.

### 2. Data Cleaning
- Handle missing values
- Remove physically impossible measurements
- Validate ranges

### 3. Feature Engineering
Generate physically meaningful variables:

- Absolute Magnitude
- Log-scaled temperature
- Luminosity representations

### 4. Exploratory Data Analysis
- HR Diagram
- Feature distributions
- Correlation analysis

---

## 🤖 Machine Learning

### Stellar Classification
Predict stellar categories using supervised learning.

Possible outputs:

- Main Sequence
- Giants
- Supergiants
- White Dwarfs

Models:
- Random Forest
- Logistic Regression
- SVM

---

### Anomaly Detection

Identify unusual stellar objects.

Methods:

- DBSCAN
- Isolation Forest

Outputs:
- Rare stars
- Extreme spectral profiles
- Unusual HR positions

---

## 🎼 Spectral → Music Mapping

The musical output is generated from stellar characteristics.

Example mapping:

| Stellar Property | Musical Parameter |
|-----------------|------------------|
| Temperature | Pitch |
| Luminosity | Volume |
| Mass | Duration |
| Stellar Class | Instrument |
| Anomaly Score | Harmony Complexity |

---

## 🛠 Tech Stack

Python

Data:
- pandas
- numpy

Visualization:
- matplotlib
- plotly

Machine Learning:
- scikit-learn

Audio:
- MIDIUtil
- FluidSynth

Deployment:
- Streamlit
- Hugging Face Spaces

---

## 🚀 Future Features

- Interactive HR diagram
- Clickable stars
- Audio playback
- Dynamic motif generation
- Real-time prediction
- Star information popups

---

## 📂 Project Structure

```text
Stellar-Spectral-Music/
│
├── data/
├── notebooks/
├── models/
├── audio/
├── app.py
├── requirements.txt
├── README.md
└── assets/
```

---

## 🎓 Motivation

Stars are usually studied visually.

This project explores a different question:

> What if stellar evolution could be heard?

By combining astronomy and machine learning, Stellar Spectral Music transforms astrophysical structure into an interactive musical experience.

---

## 📌 Status

🚧 In Development
