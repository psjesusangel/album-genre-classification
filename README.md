# Album Cover Genre Classification

**Author:** Jesus Perez Sanchez  
**Course:** CPSC 480 - Computer Vision  
**Yale University, December 2025**

## Overview

This project uses computer vision and deep learning to classify album covers into 4 musical genres (HipHop, Rock, Pop, Electronic). I compared traditional CV features covered in lecture (color, edges, texture, faces) against a CNN achieving 40.42% test accuracy.

**Components:**

- Hand-crafted CV feature extraction (25 features per image)
- Random Forest baseline (29.58% accuracy)
- ResNet-18 CNN with transfer learning (40.42% accuracy)
- Grad-CAM interpretability visualizations
- Interactive demo for exploring results (final section)

## How to Run

### 1. Open in Google Colab

**Option A:** Upload notebook directly

- Go to [colab.research.google.com](https://colab.research.google.com/)
- File → Upload notebook → Select `genre_classification.ipynb`

**Option B:** Open from GitHub

- Go to [colab.research.google.com](https://colab.research.google.com/)
- File → Open notebook → GitHub tab
- Enter: `psjesusangel/album-genre-classification`
- Select `genre_classification.ipynb`

### 2. Enable GPU

- Runtime → Change runtime type
- Hardware accelerator → **GPU (T4)**
- Save

### 3. Run the Notebook

- Runtime → Run all
- Feel free to skip visualization steps, what's most important is that the functionality blocks are ran to see results
- **Note**: Allow up to 10 minutes for the full notebook to run (much longer if ran on CPU!)

### 4. Interactive Demo (Section 11)

- **Important:** Previous cells have to be ran for this section to work; sections before this can be quite dense so feel free to use this section to get a quick idea of the project and results!
- Use the dropdown and buttons to explore different album covers
- See complete analysis: CV features → predictions → Grad-CAM → insights

## Expected Results

The notebook will produce:

- Visualizations of sample album covers
- CV feature analysis plots
- Training curves (loss & accuracy)
- Confusion matrix showing classification performance
- Grad-CAM heatmaps revealing CNN attention
- Interactive demo for exploring the system

**Test Accuracy:** 40.42% (vs. 25% random baseline, 29.58% traditional CV)

## Files

- `genre_classification.ipynb` - Complete project notebook
- `README.md` - This file
- `album_cover_report.pdf` - Full technical report (uploaded separately)

---

_Dataset: "20k-Album-Covers-within-20-Genres" from HuggingFace_  
_Random seed: 42 for reproducibility_
