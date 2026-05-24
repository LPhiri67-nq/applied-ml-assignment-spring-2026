# applied-ml-assignment-spring-2026


This repository contains the complete code and report for the **Applied Machine Learning** module assignment (University of Sussex, Spring 2026).

> **Note**: This repository is public for submission purposes only. It is **not** an open-source project.
&nbsp;

&nbsp;
## 📋 Assignment Overview

**Task 1 – Natural Language Processing (50%)**  
Binary sentiment analysis on movie reviews contaminated with randomly mixed email-style spam.

**Task 2 – Computer Vision (50%)**  
Face alignment by localising facial landmarks in images with geometric and photometric variability.
&nbsp;
&nbsp;
## 📁 Repository Structure

```text
applied-ml-assignment-spring-2026/
├── Task1_Sentiment_Analysis/
│   ├── task1_final.ipynb                 # Main notebook for Task 1
│   └── task1_predictions.csv             # Final submission file
├── Task2_Face_Alignment/
│   ├── task2_final.ipynb                 # Main notebook for Task 2
│   └── task2_predictions.csv             # Final submission file
├── Report/
│   └── report.pdf                        # Full assignment report (PDF)
├── figures/                              # Figures and diagrams used in the report
└── README.md
```
&nbsp;
&nbsp;
## 🚀 Key Features

### Task 1 – Sentiment Analysis
- Thorough EDA revealing ~25.8% spam contamination
- TF-IDF with n-grams and custom stopword handling (preserving negation)
- Hybrid spam-aware system (rule-based + confidence thresholding)
- Multiple approaches compared (Baseline, Clean-only, Spam-aware)
- External evaluation on NLTK `movie_reviews` dataset

### Task 2 – Face Alignment
- Custom CNN for landmark regression
- Comprehensive data augmentation (geometric + photometric)
- Proper landmark coordinate scaling and normalisation
- Comparison between classical (HOG + Ridge) and deep learning approaches
- Cumulative Error Distribution (CED) analysis

## 📊 Figures

All visualisations available in the notebooks and used in the report are available in the `figures/` folder:

**Task 1 – Sentiment Analysis**
- `review_length_distribution.png` — Review length distribution by sentiment class
- `confusion_matrix_baseline.png` — Confusion matrix for the baseline model
- `confusion_matrix_clean.png` — Confusion matrix for the clean-only model
- `pipeline_diagram_task1.png` — Overall sentiment analysis pipeline with spam detection

**Task 2 – Face Alignment**
- `average_face_landmarks.png` — Average face with landmark positions
- `ced_curve_all_systems.png` — Cumulative Error Distribution curves for all systems (NB: Currently not inluded in the report)
- `landmark_comparison_example.png` — Example landmark predictions (Ground Truth vs System 1 vs System 3)
- `landmark_good_example.png` — Successful landmark prediction example
- `landmark_failure_example.png` — Failure case example
- `robustness_analysis.png` — Robustness test results

## 📝 Report

The full assignment report (`MachineLearning_FinalReport.pdf`) is available in the `Report/` folder.

## Important Notes
- Original datasets are **not** included (as per assignment instructions).
- All code is self-contained and reproducible for marking purposes.
- This repository is public **only for submission convenience** and is NOT an open-source project.
