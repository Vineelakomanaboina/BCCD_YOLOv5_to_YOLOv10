# BCCD_YOLOv5_to_YOLOv10


# Project Overview
This project focuses on detecting and counting blood cells using YOLO (You Only Look Once) models on the BCCD dataset. A comparative analysis has been performed between different YOLO versions, ranging from YOLOv5 to YOLOv10, to evaluate their performance in terms of accuracy, speed, and efficiency.

# Dataset
The BCCD dataset contains annotated blood cell images for detecting and counting different types of cells, such as Red Blood Cells (RBCs), White Blood Cells (WBCs), and Platelets.

# Objective
To detect and count blood cells accurately using YOLO models.
To compare YOLOv5 to YOLOv10 based on:
Precision, Recall, and F1-Score
Inference speed (FPS)
Model size and complexity
YOLO Versions Compared
YOLOv5
YOLOv6
YOLOv7
YOLOv8
YOLOv9
YOLOv10
# Methodology
# Data Preprocessing:

The BCCD dataset images were resized to 640x640 pixels for uniformity.
Standard data augmentation techniques were applied to improve model generalization.
Model Training:

Each YOLO model was trained on the dataset using the same hyperparameters for a fair comparison.
Training was conducted in Google Colab with GPU acceleration.
Evaluation Metrics:

Precision, Recall, and F1-Score for detection performance.
Inference Speed (FPS) for real-time applicability.
Model Size to evaluate resource requirements.
# Results
# Overall Trends:
• YOLOv8 consistently performs best across blood cell types, achieving high Precision
and Recall, indicating it balances sensitivity and specificity effectively.
• YOLOv7 and YOLOv9 show competitive results, particularly in Recall and
mAP@0.5, with YOLOv9 slightly outperforming in Recall for some cases.
• YOLOv10, while performing reasonably well, scores lower across most metrics,
suggesting it may be less reliable for this dataset.
Performance by Blood Cell Type:
• Platelets: YOLOv8 achieves the highest Precision (0.828) and Recall (0.895),
accurately detecting platelets with minimal false positives. YOLOv9 also performs
well, especially in Recall (0.908), valuable for high-sensitivity needs.
• RBC (Red Blood Cells): YOLOv8 leads in Recall (0.79) and mAP@0.5:0.95 (0.634),
making it the most robust for RBC detection. YOLOv9 is close in Recall but trails
slightly in mAP@0.5:0.95.Chapter 5. Results and Discussion 27
• WBC (White Blood Cells): All models show high Precision and Recall, with
YOLOv8 and YOLOv9 achieving near-perfect scores (Precision 0.96, Recall 1.0),
ensuring reliability for WBC detection.
# Detailed Metric Analysis:
mAP@0.5:0.95, which evaluates model performance across various IoU thresholds,
highlights YOLOv8 as the top model, suggesting it balances Precision and Recall even
with variable detection requirements.
