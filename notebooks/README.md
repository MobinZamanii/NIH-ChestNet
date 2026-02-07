## 📒 Notebooks Overview

This directory contains the core experimental notebooks used to build, train, evaluate, and deploy the clinical X-ray diagnostic system.  
Each notebook corresponds to a specific phase of the machine learning pipeline.

---

### Notebook List

| Notebook | Description |
|----------|-------------|
| `01_Exploratory_Data_Analysis.ipynb` | Dataset inspection, label distribution analysis, and initial visual exploration of chest X-ray samples. |
| `02_Data_Preprocessing_and_Augmentation.ipynb` | Image preprocessing pipeline, normalization, and data augmentation strategies. |
| `03_Model_Architecture_and_Training.ipynb` | Implementation and fine-tuning of the DenseNet-121 multi-label classification model. |
| `04_Model_Evaluation.ipynb` | Performance evaluation using AUC, ROC curves, and per-class metrics. |
| `05_Final_Inference_and_Global_Evaluation.ipynb` | Batch inference pipeline, probability calibration, Grad-CAM generation, and final report creation. |

---

### Additional Files

| File | Description |
|------|-------------|
| `final_performance_report.csv` | Final evaluation metrics for all pathologies. |
| `final_summary.txt` | Text summary of model performance and clinical findings. |

---

### Recommended Execution Order

Run the notebooks in the following order:

```
01 → 02 → 03 → 04 → 05
```

This sequence represents the complete workflow:

1. Data exploration
2. Preprocessing and augmentation
3. Model training
4. Evaluation
5. Final inference and reporting

---

### Reproducibility Notes

- Ensure dependencies from `requirements.txt` are installed.
- Update dataset paths according to your local setup.
- For large-scale or production inference, use the script-based pipeline instead of notebooks.
