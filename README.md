#  Smart Classroom Attention Analyzer

## Overview
A deep learning-based system that automatically detects and analyzes 
student behaviour in classroom environments using computer vision. 
Built with EfficientNet-B0 and Transfer Learning, this model performs 
**multi-label classification** — meaning it can detect multiple 
behaviours happening at the same time in a single image.

##  Problem Statement
Manually monitoring student attention and behaviour in classrooms is 
time-consuming and subjective. This project automates that process 
using AI, helping educators identify engagement levels and 
behavioural patterns at scale.

## Dataset
- **Source:** Student Behaviour Detection (Roboflow)
- **Size:** 4,065 images
- **Classes:** 12 behaviour labels

##  Behaviour Classes Detected
| Label | Description |
|-------|-------------|
| `upright` | Student sitting upright |
| `writing` | Student writing |
| `reading` | Student reading |
| `book` | Student holding/using a book |
| `hand-raising` | Student raising hand |
| `raise_head` | Student raising their head |
| `bow_head` | Student bowing their head |
| `turn_head` | Student turning their head |
| `sleep` | Student sleeping |
| `bend` | Student bending |
| `phone` | Phone visible |
| `Using_phone` | Student actively using phone |

##  Model Architecture
- **Base Model:** EfficientNet-B0 (pretrained on ImageNet)
- **Approach:** Transfer Learning with fine-tuning
- **Task:** Multi-label image classification
- **Framework:** PyTorch

##  How It Works
1. Images are captured from the classroom
2. EfficientNet-B0 extracts visual features
3. The model outputs probabilities for all 12 behaviour labels
4. Multiple behaviours can be flagged simultaneously per image

##  Getting Started
1. Open the notebook in **Google Colab**
2. Set runtime to **T4 GPU**
3. Upload the dataset zip file
4. Run all cells sequentially

##  Tech Stack
- Python
- PyTorch & TorchVision
- EfficientNet-B0
- scikit-learn
- Matplotlib & Seaborn
- Google Colab
