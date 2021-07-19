# pstage_02_image_classification

## Getting Started

### Dependencies

- torch==1.6.0
- torchvision==0.7.0

### Install Requirements

- `pip install -r requirements.txt`

### Training

- `SM_CHANNEL_TRAIN=[train image dir] SM_MODEL_DIR=[model saving dir] python train.py`

### Inference

- `SM_CHANNEL_EVAL=[eval image dir] SM_CHANNEL_MODEL=[model saved dir] SM_OUTPUT_DATA_DIR=[inference output dir] python inference.py`

### Evaluation

- `SM_GROUND_TRUTH_DIR=[GT dir] SM_OUTPUT_DATA_DIR=[inference output dir] python evaluation.py`

## Models

- VGG-19
- ResNet50
- FaceNet
- EfficientNet b7

## Experiment

18 class 를 하나의 모델로 실험 + 3개로 나누어 실험

- age (30↓, 30~60, 60↑)
- mask (wear, incorrect, not wear)
- gender (male, female)
