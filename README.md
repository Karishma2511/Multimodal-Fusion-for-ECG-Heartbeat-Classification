**Multimodal Fusion for ECG Heartbeat Classification
**
This project focuses on leveraging multimodal fusion techniques to classify ECG heartbeats into Normal and Myocardial Infarction categories using advanced pre-processing and deep learning methodologies.

**Overview
**
Electrocardiograms (ECG) are critical for diagnosing cardiac conditions. Using the PTB Diagnostic ECG Database, we transformed raw ECG signals into image representations using:

Gramian Angular Field (GAF)

Markov Transition Field (MTF)

Recurrence Plot (RP)

We developed two classification frameworks:

Multimodal Image Fusion (MIF): Combines image modalities into a single input.

Multimodal Feature Fusion (MFF): Extracts features independently from modalities and fuses them using a Gated Fusion Network (GFN).

**Key Features
**
Signal Preprocessing: Converts ECG signals into image representations.

Deep Learning Models: Implements MIF and MFF frameworks for classification.

Gated Fusion Network (GFN): Optimizes feature integration dynamically.

Performance: Achieves 98% accuracy with the MIF framework.

**Steps and Workflow
**
1. Create GAF, RP, and MTF Images

Transformed ECG signals into temporal, probabilistic, and recurrence-based image modalities.

Tools: pyts.image, NumPy.

2. Dataset Creation

Created a structured dataset containing the GAF, RP, and MTF images.

Balanced classes to ensure robust model training.

3. Build MIF (Multimodal Image Fusion) Model

Combined image modalities into a single triple-channel input.

Trained using CNN architectures for feature extraction and classification.

4. Build MFF (Multimodal Feature Fusion) Model

Extracted features independently from each modality using pre-trained models (e.g., AlexNet).

Integrated features dynamically with a Gated Fusion Network (GFN).

5. Integration

Unified the pipeline for image input, feature extraction, fusion, and classification.

Optimized GFN for dynamic feature weighting and computational efficiency.

6. Testing and Evaluation

Evaluated models on accuracy, precision, recall, and F1-score.

Compared MIF and MFF frameworks to identify the optimal approach.

**Technologies and Tools Used
**
Programming Languages: Python

Libraries: NumPy, Pandas, Matplotlib, PyTS, TensorFlow, Keras

Pretrained Models: AlexNet

Tools: Jupyter Notebook, Matplotlib, Scikit-learn

**Results
**
Multimodal Image Fusion (MIF): 98% classification accuracy.

Multimodal Feature Fusion (MFF): Enhanced interpretability and computational efficiency.

**Future Work
**
Extend the dataset with more diverse cardiac conditions.

Explore additional modalities for richer feature extraction.

Optimize real-time deployment for clinical use.
