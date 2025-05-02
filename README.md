[Model-Accuracy-Precision-Recall-AUC.csv](https://github.com/user-attachments/files/20011073/Model-Accuracy-Precision-Recall-AUC.csv)Project 1 : Vision Transformer-Based Analysis of Handwritten Text for Early Dyslexia Detection in Children


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


Project 2 : Continuous Analysis of Autism Spectrum Disorder Using Advanced Deep Learning Approach for Gradient-Based Classification


Overview
This project focuses on the development and evaluation of advanced deep learning models for the automated detection and continuous analysis of Autism Spectrum Disorder (ASD) using facial images and behavioral data. ASD is a complex neurodevelopmental condition with a wide spectrum of behavioral, cognitive, and social manifestations, making early and accurate diagnosis challenging. The project leverages state-of-the-art deep learning architectures, including convolutional neural networks (CNNs), recurrent neural networks (RNNs), and attention mechanisms, to improve the specificity, accuracy, and interpretability of ASD classification.


What the Project Does
Automated ASD Detection: Implements a suite of pre-trained deep learning models (VGG19, VGG16, XceptionNet, MobileNetV2, InceptionV3, ResNet50) for classifying individuals as autistic or non-autistic based on facial images.

Gradient-Based Classification: Introduces a novel gradient-based classification algorithm that enhances the granularity and accuracy of ASD spectrum analysis, enabling more detailed and personalized diagnostic insights.

Multimodal Data Integration: Incorporates behavioral, cognitive, and genetic data where available, allowing for a richer and more nuanced representation of ASD traits.

Severity Estimation: Provides not only binary classification but also estimates the severity of autism (mild, moderate, severe) based on model confidence scores.

Performance Evaluation: Utilizes comprehensive metrics-accuracy, precision, recall, F1-score, ROC-AUC, and confusion matrices-to rigorously assess model performance and generalizability.

Key Contributions
Comprehensive Model Benchmarking: Systematically evaluates six leading deep learning architectures for ASD detection, identifying strengths and trade-offs in accuracy, computational efficiency, and robustness.

Transfer Learning for Medical Imaging: Demonstrates the effectiveness of transfer learning by fine-tuning ImageNet-pretrained models on ASD datasets, significantly improving classification performance even with limited data.

Object Detection Integration: Employs object detection (MobileNet-SSD) to localize facial regions in images, ensuring the models focus on the most informative features for ASD diagnosis.

Open, Scalable Framework: Provides a reproducible pipeline for ASD screening that can be adapted for deployment in clinical, educational, or mobile health settings.

Methodology
Data Preparation: Images are resized to 224x224 pixels, and object detection is used to focus on facial regions. The dataset is split into training (80%), validation (10%), and testing (10%) sets.

Model Training: Each deep learning model is loaded with pre-trained weights, with custom classification layers added and fine-tuned for the ASD detection task. Training uses categorical cross-entropy loss and the Adam optimizer, with early stopping and model checkpointing.

Evaluation: Model performance is tracked across epochs using accuracy and loss curves, with final evaluation based on precision, recall, F1-score, ROC-AUC, and confusion matrices.

Severity Prediction: The system outputs confidence scores for each prediction, which can be mapped to severity levels for ASD (e.g., >90% severe, 70–90% moderate, <70% mild).

Results
Model	 Accuracy	Precision	Recall	AUC
VGG19	0.77	0.77	0.78	0.77
VGG16	0.78	0.78	0.77	0.78
XceptionNet	0.83	0.83	0.83	0.83
MobileNetV2	0.81	0.81	0.81	0.81
InceptionV3	0.79	0.79	0.79	0.79
ResNet50	0.85	0.85	0.85	0.85
Best Performance: ResNet50 achieved the highest test accuracy (85%), precision, recall, and AUC, making it the most robust model for ASD detection in this study.

Severity Estimation: The model provides a confidence-based estimation of ASD severity, supporting more nuanced clinical interpretation.

Generalization: The use of transfer learning and data augmentation improved the models' ability to generalize to new, unseen data.

Impact
Clinical and Educational Utility: Offers a scalable, non-invasive, and accurate tool for early ASD screening, supporting clinicians and educators in timely intervention and personalized care.

Research Advancement: Sets a benchmark for the application of deep learning and transfer learning in neurodevelopmental disorder detection, with a reproducible and extensible framework for future studies.

References
For detailed methodology, implementation, and results, see the full paper: Continuous Analysis of Autism Spectrum Disorder Using Advanced Deep Learning Approach for Gradient-Based Classification by Ayan Sar, Sumit Aich, Pranav Singh, Tanupriya Choudhury, Hussain Falih Mahdi.
