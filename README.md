## AI-Powered Clinical X-Ray Diagnostic System

An end-to-end deep learning pipeline for multi-label classification of 14 chest pathologies from frontal chest X-ray images.  
This project evolves from raw data training to a calibrated, explainable, and automated clinical reporting system.

---

### Project Highlights

**Architecture**
- Fine-tuned **DenseNet-121** backbone
- Global Average Pooling head
- Multi-label sigmoid output for 14 pathologies

**Explainability (XAI)**
- Integrated **Grad-CAM** visualization
- Heatmap overlays to verify model attention regions
- Clinically interpretable outputs

**Clinical Reliability**
- **Probability calibration** applied post-training
- Reduced overconfidence in predictions
- Improved Expected Calibration Error (ECE)

**Automation**
- Batch inference engine
- Structured **CSV clinical report generation**
- Scalable processing for hundreds of X-ray images

---

### Performance Metrics

The model demonstrates expert-level discrimination ability across several critical pathologies.

| Pathology      | AUC Score |
|----------------|----------|
| Cardiomegaly   | 0.926    |
| Emphysema      | 0.922    |
| Pneumothorax   | 0.901    |
| Effusion       | 0.897    |
| **Average AUC**| **0.844**|

---

### Reliability Calibration

Post-training probability calibration significantly reduced the **Expected Calibration Error (ECE)**.

- Near **0.00% ECE** across most classes
- Improved probability reliability
- Reduced model overconfidence
- Better alignment with real clinical prevalence

---

### Visual Evidence (Grad-CAM)

The system not only predicts pathologies but also provides visual explanations.

**Workflow:**
1. Input: Standard frontal chest X-ray
2. Model prediction
3. Grad-CAM heatmap generation
4. Overlay visualization highlighting suspicious regions

**Output:**
- Red/Yellow heatmaps indicate regions responsible for positive predictions
- Supports clinical interpretability and model trust

---

### Key Features

- **Automated Reporting**
  - Processes entire image directories
  - Exports `final_clinical_report.csv`

- **Statistical Dashboard**
  - Pathology distribution charts
  - Frequency bar plots and pie charts

- **Real-time Progress Tracking**
  - Integrated `tqdm` for batch inference

- **XAI Visualizer**
  - Automatic Grad-CAM heatmap generation
  - Saved per detected abnormality

---

### System Pipeline

```
Raw X-ray Images
        ↓
Preprocessing & Normalization
        ↓
DenseNet-121 Multi-Label Classifier
        ↓
Probability Calibration
        ↓
Grad-CAM Explainability
        ↓
Batch Inference Engine
        ↓
CSV Clinical Report + Visual Outputs
```


---

### Tech Stack

- Python
- PyTorch
- Torchvision
- NumPy / Pandas
- Matplotlib / Seaborn
- OpenCV
- tqdm

---

### Clinical Disclaimer

This project is a **research-grade AI system** intended for academic and experimental purposes only.  
It is **not approved for clinical deployment** and must not be used as a substitute for professional medical diagnosis.
