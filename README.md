# CytologIA Data Challenge: Advancing Hematological Diagnostics Through AI

## Overview

Welcome to the official repository for the **CytologIA Data Challenge**, hosted on [Trustii.io](https://app.trustii.io). This challenge ran from **November 25, 2024** to **January 6, 2025** and brought together data scientists from around the globe to tackle an ambitious goal: **automating the detection and classification of leukocytes in blood smear images**.

- **`README.md`** (this document)  
  Provides a high-level summary of the challenge and the winning solutions.

### Quick Facts

- **Participants**: 245 (worldwide)  
- **Submissions**: 1,958 total, peaking in the final three days  
- **Dataset**: ~69,000 images, 23 classes of leukocytes (normal & pathological)  
- **Total Prize**: €25,000 awarded to the top 3 solutions  
- **Final Leaderboard**: Extremely tight competition, with scores >0.93 for the top 9 entries

## Challenge Background

### Hematology & The Motivation
Hematology critically relies on analyzing blood smears to identify and classify white blood cells (leukocytes). Historically, this involves **manual microscope inspection**, which is time-consuming and demands specialized expertise. While automated counters exist, their classification performance often falls short in complex or atypical cases.

By **harnessing AI** for blood smear analysis, the CytologIA project aims to:
1. **Standardize** diagnostic practices across diverse regions and laboratories.
2. **Improve** the accuracy and speed of leukocyte classification.
3. **Foster** open, collaborative research in medical imaging.

### Project Partners
- **French Cellular Hematology Group** (GFHC), comprising ~300 hematologists.
- **Algoscope**, an imaging and AI solutions provider.
- **Supported by France 2030** in partnership with the **Health Data Hub**.
- **Trustii.io**, the platform hosting the challenge and leaderboards.

### The Dataset
- **23 Leukocyte Classes** with at least 1,000 images each.
- **Diverse Resolutions**, commonly 370×368 pixels.
- **~69,000 Images** total, covering both normal and pathological cells.
- **Expert Annotation** by experienced cytologists.
- **Multicentric** input to ensure variability and reduce overfitting risk.

## Results & Winners

> **Winners Announced**: End of January 2025  

After thorough validation and private leaderboard scoring, three solutions emerged at the top. **All three** repositories are included here as Git submodules, along with their detailed reports in the `reports/` folder.

### 1. **MPWARE – 1st Place**
- **Key Approach**: Two-stage pipeline using YOLOX for detection and CNN/Transformers for classification.  
- **Highlights**:  
  - Exceptionally **well-documented** notebooks for data prep, training, and inference.  
  - Innovative pipeline maximizing performance across varied data scenarios.  
- **Repo**: [MPWARE Team GitHub](https://github.com/MPWARE-TEAM/Cytologia/tree/main)

### 2. **Xueer – 2nd Place**
- **Key Approach**: An **ensemble** of 16 models (4 detection + 12 classification), leveraging diverse augmentations.  
- **Highlights**:  
  - Uses modern YOLOv9 and YOLOv11 architectures.  
  - Probability averaging to merge model outputs effectively.  
- **Repo**: [Xueer Chen GitHub](https://github.com/xueerchen1990/cytologia_2nd_place)

### 3. **Simon Thomine – 3rd Place**
- **Key Approach**: A single-step YOLO model for **both** detection and classification of 23 classes.  
- **Highlights**:  
  - Emphasizes data cleaning and **annotation quality**.  
  - Straightforward pipeline with detailed, structured documentation.  
- **Repo**: [Simon Thomine GitHub](https://github.com/SimonThomine/Cytologia-Data-Challenge)

## Repository Contents

- **`reports/`**  
  PDF files detailing each winner’s method, including data processing, model architecture, training strategies, and inference steps.
  
- **Submodules**  
  - `MPWARE/` – (1st Place)  
  - `Xueer/` – (2nd Place)  
  - `Simon_Thomine/` – (3rd Place)  

## How to Get Started

1. **Clone This Repo (with Submodules)**
   ```bash
   git clone --recursive https://github.com/Trustii-io/cytologia-challenge-results.git

## Who to contact

If you have any question about this data challenge, you can reach out to us at challenges@trustii.io.

Also, you can find the complete notebooks submitted during the challenge at https://app.trustii.io / the cytologia challenge private leaderboard
