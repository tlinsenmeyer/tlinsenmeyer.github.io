---
layout: home
title: "Occupancy Modeling"
---


# Predictive Occupancy Modeling

This project uses environmental sensor data to predict room occupancy. The dataset included sound, temperature, light, CO₂, and PIR motion readings. The goal was to determine whether sensor data alone could reliably estimate how many people were in a room.

---

## What I Did

- Cleaned and explored a 10,000‑row sensor dataset  
- Engineered new features (average temp, light, sound, PIR)  
- Ran PCA to understand dimensionality  
- Evaluated multiple machine learning models  
- Accelerated SVM training using CUDA on a GPU  

---

## Models Tested

- Linear Regression  
- K‑Nearest Neighbors  
- Random Forest  
- Support Vector Machine (CPU + GPU)  

The SVM model performed the best once GPU acceleration was used, reducing training time from over an hour to six seconds.

---

## Key Findings

- Linear models struggled due to non‑linear relationships  
- KNN and Random Forest improved generalization  
- SVM with RBF kernel provided the strongest performance  
- GPU acceleration was essential for practical training times  

---

## Why This Project Matters

Accurate occupancy prediction can improve HVAC efficiency, reduce energy waste, and support smart‑building automation. This project shows how machine learning can be applied to real operational problems.

[View this Project Notebook (via nbviewer)](https://nbviewer.org/github/tlinsenmeyer/estimate_occupancy/blob/main/estimate_occupancy.ipynb)

---

<p align="center" style="color:#C0C0C0; font-size: 0.9em;">
  <span style="color:#00AEEF;">●</span>
  Engineering • Simulation • Machine Learning
  <span style="color:#00AEEF;">●</span><br>
  <span style="color:#2EC4B6;">Designing Smarter Systems</span><br><br>
  <span style="color:#777777;">© 2026 Tom Linsenmeyer</span>
</p>




