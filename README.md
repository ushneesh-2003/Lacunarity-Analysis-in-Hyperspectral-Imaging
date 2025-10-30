# 🌌 Lacunarity Analysis in Hyperspectral Imaging

![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)
![License](https://img.shields.io/badge/license-CC%20BY--NC--SA%204.0-lightgrey.svg)
![Remote Sensing](https://img.shields.io/badge/Domain-Remote%20Sensing-blueviolet.svg)

This repository presents the implementation and analysis framework for **Lacunarity Analysis in Hyperspectral Imaging**, a study focused on quantifying **spatial heterogeneity** in hyperspectral data using **gliding box lacunarity**.  
The project investigates the **Indian Pines** dataset, emphasizing **Band 29** as the maximum information band, and provides a robust statistical foundation for texture-based spatial analysis in hyperspectral imagery.

---

## 🧩 Overview

**Objective:**  
To utilize **lacunarity** as a statistical measure for assessing **image heterogeneity** across multiple **Regions of Interest (ROIs)** in hyperspectral data.

**Key Highlights:**
- Identifies **Band 29** as the “maximum information band” using standard deviation analysis.  
- Applies **gliding box lacunarity** to study texture variation at multiple scales.  
- Demonstrates spatial heterogeneity trends across four ROIs, revealing complex structural and textural differences.  
- Establishes lacunarity as a reliable metric for **land cover differentiation**, **texture interpretation**, and **scale-dependent variability** in hyperspectral imagery.

---

## 🧠 Methodology

1. **Band Selection:**  
   - Computed the standard deviation across all spectral bands in Indian Pines.  
   - Selected **Band 29** as it showed the highest variance (most informative).

2. **Gliding Box Lacunarity Computation:**  
   - Applied sliding window analysis across four ROIs.  
   - Calculated lacunarity (Λ) using variance-based equations for each box size.

3. **Equations Used:**
   \[
   σ^2 = \frac{\sum(x_i - μ)^2}{N}
   \]
   \[
   Λ = \frac{σ^2}{μ}
   \]
   \[
   Λ_{mean} = \frac{\sum Λ_{ij}}{M}
   \]

4. **Multi-Scale Analysis:**  
   - Window sizes varied from small (2×2) to large (32×32).  
   - Observed scale-dependent variations in spatial texture.

---

## 📊 Results Summary

| ROI | Land Cover Types | Lacunarity Pattern | Texture Description |
|-----|------------------|--------------------|---------------------|
| ROI 1 | Alfalfa, Corn-Notill, Corn-Mintill | High & Consistent | Highly heterogeneous |
| ROI 2 | Alfalfa, Woods | Moderate, Decreasing | Structured, organized texture |
| ROI 3 | Woods, Alfalfa, Soybean-Mintill | High, Decreasing | Complex and irregular |
| ROI 4 | Soybean-Mintill, Alfalfa | Moderate-High | Textured, uneven pattern |

- **ROI 1**: Highest lacunarity → complex land cover mix.  
- **ROI 2**: Declining trend → organized pattern.  
- **ROI 3**: High variability → multi-component structure.  
- **ROI 4**: Moderate heterogeneity → agricultural blend.

---

## 🧮 Technical Insights

- **Algorithm:** Variance-based gliding box method  
- **Complexity:** \(O(n \times m)\), where *n* = pixels, *m* = scales analyzed  
- **Advantages:**
  - Sensitive to local texture changes  
  - Efficient for large hyperspectral datasets  
  - Captures scale-dependent structural variations

---

## 🌍 Applications

- Remote sensing & land cover classification  
- Ecological and environmental modeling  
- Agricultural monitoring  
- Urban planning and spatial complexity studies  
- Integration with **machine learning** and **fractal feature extraction**

---

## 📘 Citation

If you use this work, please cite:

**Anindita Das Bhattacharjee, Ushneesh Chattopadhyay, Sayani Basu, and Arjo Bhattacharya**  
*Lacunarity Analysis in Hyperspectral Imaging*,  
Institute of Engineering and Management (IEM), Kolkata, India, 2025.

---

## 📜 License

This project is licensed under the  
[**Creative Commons Attribution–NonCommercial–ShareAlike 4.0 International License (CC BY-NC-SA 4.0)**](https://creativecommons.org/licenses/by-nc-sa/4.0/).

You may copy, remix, and build upon the material **for non-commercial purposes only**,  
with proper credit and under the same license.

---

## 👩‍💻 Contributors

- **Anindita Das Bhattacharjee** – IEM Centre of Excellence for InnovAI  
- **Ushneesh Chattopadhyay** – Institute of Engineering and Management  
- **Sayani Basu** – Institute of Engineering and Management  
- **Arjo Bhattacharya** – Institute of Engineering and Management  

---

## 📬 Contact

For questions or collaborations:  
📧 [chattopadhyayushneesh2003@gmail.com](mailto:chattopadhyayushneesh2003@gmail.com)
