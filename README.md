# Circular Aperture Antenna Radiation Pattern Analyzer

**A Python-based visualization and analysis tool for the radiation pattern of a uniformly illuminated circular aperture antenna (D = λ).**


<img width="1168" height="672" alt="image" src="https://github.com/user-attachments/assets/d150a4e0-5989-477c-8dd5-df50f68cbd77" />
<img width="908" height="757" alt="image" src="https://github.com/user-attachments/assets/b07f00d9-d991-4f2e-a88a-5eb2628244ba" />
<img width="915" height="547" alt="image" src="https://github.com/user-attachments/assets/4817508e-7a3d-4589-a8fa-a5ca80a7dcbd" />

---

## Introduction

This project analyzes and visualizes the far-field radiation pattern of a **circular aperture antenna** with diameter equal to one wavelength (D = λ). 

Using fundamental antenna theory, the tool computes the normalized radiation pattern based on the Bessel function of the first kind and provides clear, publication-quality visualizations in both 2D and 3D. It is designed as an educational and engineering tool to help students and researchers better understand aperture antenna behavior, beamwidth, nulls, and side lobes.

Built in Python and optimized for **Google Colab**, the project offers interactive and insightful visualizations suitable for antenna theory coursework and reports.

---

## Key Features

- Accurate computation of the normalized radiation pattern \( F(\theta) \)
- High-quality **2D Polar Plots** in both linear and decibel (dB) scales
- **3D Surface Plot** showing rotational symmetry about the z-axis
- **Rectangular Diagram (RD)** with clearly marked key features
- Automatic calculation and display of:
  - Main lobe direction
  - First null location
  - Half-Power Beamwidth (HPBW)
  - First side lobe level and location
- Professional annotations and visual markers on all plots
- Robust numerical handling (avoids division by zero at θ = 0°)

---

## Mathematical Background

The normalized radiation pattern for a uniformly illuminated circular aperture is given by:

\[
F(\theta) = \left| \frac{2 J_1(2\pi \sin\theta)}{2\pi \sin\theta} \right|
\]

where \( J_1 \) is the Bessel function of the first kind of order one.  

This expression produces the characteristic "Airy disk" pattern with a dominant main lobe and decaying side lobes. The first null occurs where \( J_1(x) = 0 \), and the pattern exhibits perfect rotational symmetry due to the circular geometry of the aperture.

---

## Technologies Used

- **Python 3**
- **NumPy** – Numerical computations
- **SciPy** – Bessel function evaluation (`scipy.special.j1`)
- **Matplotlib** – 2D and 3D visualization
- **Google Colab** – Interactive development and execution

---

## Visualizations and Results

The project produces four main visualizations:

1. **Polar Plot (Linear Scale)** – Shows the normalized amplitude pattern
2. **Polar Plot (dB Scale)** – Highlights dynamic range and side lobe levels
3. **3D Surface Plot** – Illustrates rotational symmetry about the z-axis
4. **Rectangular Diagram (Cartesian)** – Displays the pattern with key features clearly marked (Main Lobe, First Null, HPBW, and Side Lobe)

Key results for D = λ:
- **First Null**: ≈ 49.4°
- **Half-Power Beamwidth (HPBW)**: ≈ 68.8°
- **First Side Lobe**: Located after the first null with reduced amplitude

All plots include professional titles, labels, legends, and helpful annotations.

---

## Project Structure
