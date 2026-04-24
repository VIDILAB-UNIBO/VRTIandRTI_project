# Validating VRTI: Point Cloud Analysis and Human Perception in Paleontological Documentation

[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

--- 

## Authors and affiliation 
University of Bologna 
* Luisa Ammirati
* Alice Bordignon
* Michela Contessi
* Francesca Fabbri
  
--- 

## Project Overview
This repository contains a comprehensive analytical workflow designed to evaluate and compare two digital documentation methodologies: **Traditional RTI** (Reflectance Transformation Imaging) and **VRTI** (Virtual RTI, derived from 3D structured light scanning).

The study focuses on how different visualization mediums affect human perception and manual tracing accuracy in paleontological contexts. By converting student-produced tracings into spatial data (Point Clouds), we implement a custom Python pipeline to quantify geometric precision, interpretative consistency, and lighting preferences.
For a detailed breakdown of the experimental design, participant recruitment, and the step-by-step procedure, please refer to our official protocol:

👉 **[Experimental Protocol on Protocols.io](https://www.protocols.io/view/comparative-assessment-protocol-of-readability-usi-kqdg3m1mzl25/v1)**

---

## Workflow Structure
The analysis is organized into six logical sections:

1.  **Data Conversion**: Automated extraction of XYZ data from manual raster tracings using BGR color masking.
2.  **Quantitative Metrics**: Grid-based subsampling and spatial deviation calculation (Unidirectional RMSE).
3.  **Statistical Validation**: Normality testing (Shapiro-Wilk) and non-parametric comparison (Mann-Whitney U).
4.  **Qualitative Evaluation**: Integration of expert Likert-scale feedback to assess "Technological Transparency".
5.  **Lighting Perspective**: Analysis of user-selected "optimal" lighting coordinates to evaluate spatial behavior.
6.  **Conclusions**: Synthesis of human-centric and technology-centric findings.

---

## Methodology Highlights

### Technological Transparency
A core finding of this research is the concept of **Technological Transparency**. Our statistical analysis ($p > 0.05$) demonstrates that operators achieved comparable geometric precision regardless of the medium. The "human factor"—subjective interpretation and experience—proved to be a more significant variable than the choice between real RTI or synthetic VRTI.

### Unidirectional vs. Bidirectional Metrics
To avoid penalizing intentional paleontological omissions, we adopted **Unidirectional RMSE** as the primary metric. However, the inclusion of **Chamfer Distance** as a secondary check confirmed that while participants were more "hesitant" in complex areas, this behavior was consistent across both technologies, further validating VRTI as a reliable proxy.

---
