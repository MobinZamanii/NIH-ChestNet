1. Training Performance & Statistical Foundation
"I focused on building a solid training foundation for this model. These charts represent the learning journey of my system on the NIH ChestX-ray14 dataset."

Figure 00 & 02: Dataset Insights & Ranking > "I analyzed the class distribution to handle data imbalance. My model achieved an AUC of 0.93 for Cardiomegaly, which stands as my highest performing category, surpassing common clinical benchmarks."

Figure 01: The Confusion Matrix > "I generated this matrix to deeply understand the model's classification behavior across 14 labels, allowing me to fine-tune the balance between sensitivity and specificity."

Figure 03: Intelligence Growth > "In this chart, I tracked the Loss and AUC during fine-tuning. You can see the steady convergence, proving that my model is learning robust features without overfitting."

2. Clinical Reliability (My Calibration Work)
"One of the most important parts of my project was making the AI 'trustworthy' for doctors."

Figure 05: Probability Calibration > "I implemented post-training calibration to fix 'overconfidence' issues. By comparing the 'Before' (Red) and 'After' (Green) states, I ensured that when my model predicts a 90% probability, it actually reflects a 90% clinical reality."

3. Explainability (The 'Why' Behind the Prediction)
"I didn't want my model to be a 'black box.' I used Grad-CAM to make the AI explain its decisions visually."

Figure 04, 06 & GCAM Samples: Visual Evidence > "In these examples, you can see how my model 'thinks.' For Cardiomegaly, it highlights the heart borders. For Infiltration, it correctly scans the lung tissue. This provides the 'Visual Evidence' a radiologist needs to verify the AI’s findings."

GCAM_00013778_003 / GCAM_00013774_053 > "I tested the model against clinical noise like 'Portable' labels and medical tubes. I am proud that the model ignores these distractions and stays focused on the biological abnormalities."

4. Automated Reporting (Final Product)
"I transformed the model into a fully automated tool for hospital environments."

Figure 07: Batch Analytics > "I built a pipeline to process 100 random patients at once. This pie chart shows my automated 'Triage' results, where the system successfully categorized cases into 'Healthy' and 'Potential Findings' for doctor prioritization."
