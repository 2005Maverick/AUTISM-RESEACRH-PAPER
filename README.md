Vision Transformer-Based Analysis of Handwritten Text for Early Dyslexia Detection in Children
Overview
This project presents an AI-driven framework for the early screening of dyslexia in children through the analysis of handwritten text images using Vision Transformer (ViT) models. Dyslexia is a prevalent neurodevelopmental disorder that impairs reading and writing skills. Early detection is crucial for timely intervention, yet traditional diagnostic methods are often subjective, time-consuming, and inaccessible. This work leverages advanced computer vision and deep learning techniques to provide an objective, scalable, and automated solution for dyslexia screening based on handwriting patterns.

What the Project Does
Automated Dyslexia Screening: Utilizes Vision Transformer models to classify handwriting samples as dyslexic or non-dyslexic, enabling early and objective identification of at-risk children.

Handwriting Feature Extraction: Employs ViT's self-attention mechanism to capture both local and global features in handwriting, identifying subtle dyslexia-specific markers such as inconsistent letter sizing, irregular spacing, and alignment issues.

Data Augmentation: Implements robust data augmentation techniques (random cropping, horizontal flipping) to address the scarcity of labeled dyslexia handwriting datasets and improve model generalization.

Comprehensive Evaluation: Assesses model performance using metrics such as accuracy, precision, recall, F1-score, and ROC-AUC, ensuring reliability and robustness across diverse handwriting samples.

Key Contributions
Novel Application of Vision Transformers: First to apply ViT models for dyslexia detection from handwriting, outperforming traditional CNN-based approaches in feature extraction and classification accuracy.

Scalable and Reproducible Pipeline: Provides a workflow from data preprocessing and augmentation through model training and evaluation, suitable for deployment in educational and clinical settings.

Detailed Performance Reporting: Achieves high classification accuracy (test accuracy of 92.39%), with strong precision, recall, F1-score, and AUC metrics across all handwriting classes (A-Z), demonstrating the model's effectiveness and generalizability.

Methodology
Data Preparation: Handwriting images are preprocessed, normalized to 
224
×
224
224×224 pixels, and augmented to increase dataset diversity.

Model Architecture: Fine-tunes a pre-trained ViT-Base-Patch16 model with a custom classification head for 26 handwriting classes.

Training: Uses cross-entropy loss, Adam optimizer, learning rate scheduling, and mixed-precision training for efficiency.

Evaluation: Validates on separate test sets with detailed metric reporting and visualization (loss/accuracy curves, confusion matrices, PR and ROC curves).

Deployment: Final trained model is saved for reproducibility and potential integration into real-world screening tools.

Results
| Metric         | Validation | Testing   |
|----------------|------------|-----------|
| Accuracy       | 92.64%     | 92.39%    |
| Precision      | 91.85%     | 91.72%    |
| Recall         | 92.64%     | 92.39%    |
| F1-Score       | 92.24%     | 92.08%    |
| ROC-AUC        | 0.975      | 0.973     |
High and consistent performance across all classes, with minimal overfitting.

Reliable detection of dyslexia-specific handwriting patterns, supporting early intervention in educational and healthcare environments.

Impact
Educational and Clinical Utility: Offers a scalable, low-cost, and accurate tool for dyslexia screening, potentially improving learning outcomes and self-esteem for affected children.

Research Advancement: Demonstrates the power of transformer-based models for complex visual pattern recognition in cognitive assessment tasks.

References
For detailed methodology, results, and implementation details, see the full paper: Vision Transformer-Based Analysis of Handwritten Text for Automated Dyslexia Screening by Sumit Aich, Pranav Singh, Hussain Falih Mahdi, Ayan Sar, and Tanupriya Choudhury
