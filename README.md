# Road Condition Foundation Model

This repository contains the code, model architecture, and pretrained weights for the **Road Condition Foundation Model**, designed to improve road condition assessment through adaptive feature refinement. The model is trained on diverse datasets capturing road conditions from different perspective views, enabling robust generalization across varying environments.

## 🚀 Key Features
- **Foundation Model for Road Condition Monitoring:** Generalizes well across different environments and road types.
- **Multi-Perspective Learning:** Trained on datasets with top-down, oblique, and frontal views for comprehensive assessment.
- **Adaptive Feature Refinement:** Enhances object detection performance for fine-grained pavement defect localization.
- **Pretrained Weights:** Available for fine-tuning on domain-specific datasets or zero-shot learning applications.

---

## 📦 Repository Structure
Model architecture with adaptive feature refinement ├── model.py 
Training script for model optimization├── run train.py 
Pretrained model weights ├── pretrained/
This documentation└── README.md 

## 🏗️ Model Architecture
The model is built on an enhanced object detection framework with:
- **Adaptive Feature Enhancement Modules** for contextual understanding.
- **Improved Spatial Attention Mechanisms** to detect overlapping pavement defects.
- **Multi-perspective data support** for better generalization across real-world conditions.

---

## 📥 Installation

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/JoshuaKAsamoah/road-condition-foundation-model.git
   cd road-condition-foundation-model


2. Training the Model:
   ```bash
   python train.py --config configs/train_config.yaml

3. Inference with Pretrained Weights:
   ```bash
   python predict.py --weights pretrained/model_weights.pt --mode inference

4. Fine-Tuning for Custom Dataset:
   ```bash
   python train.py --weights pretrained/model_weights.pt --config configs/fine_tune.yaml

## 📊 Datasets
The model was trained on diverse datasets capturing:

17 road condition types, including surface defects, structural failures, and roadside hazards.
Multi-perspective views, such as top-down aerial images, oblique roadside captures, and frontal vehicle-mounted images.
You can prepare your custom datasets by following the instructions in the datasets/ directory.

### 📦 Pretrained Weights
Pretrained model weights are available here.

You can use these weights for:

Fine-tuning on domain-specific data

Zero-shot learning applications
