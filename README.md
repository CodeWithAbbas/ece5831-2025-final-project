# ECE 5831 - Speaker Recognition Final Project

## Overview
A deep learning speaker recognition system using LSTM neural networks with MFCC features. This project explores model performance across different datasets and discovers critical device bias issues in audio machine learning models.

## Project Highlights
- **LSTM-based Classification**: Deep neural network for speaker identification
- **MFCC Feature Extraction**: Mel-frequency cepstral coefficients for audio processing
- **Multi-Phase Experimentation**:
  - Phase 1: Baseline with Kaggle dataset
  - Phase 2: YouTube public figures dataset
  - Phase 3: Custom recordings (device bias discovery)
  - Phase 4: Same-device solution (solving device bias)

## Key Finding
**Device Bias Discovery**: Models trained on one recording device showed poor performance on different devices due to device-specific audio characteristics. Implemented a same-device training strategy that achieved cross-device generalization.

## Technologies
- Python
- TensorFlow/Keras
- Librosa (audio processing)
- NumPy, Pandas
- Matplotlib, Seaborn

## Repository Contents
- `final-project.ipynb` - Complete project notebook with all phases
- `speaker_recognition_final_report.pdf` - Detailed project report
- `Speaker_Recognition_Presentation.pptx` - Project presentation
- `models/` - Trained LSTM models
- `notebook_images/` - Visualization outputs
- `test_recordings/` - Sample test audio files

## Results Summary
| Phase | Dataset | Validation Accuracy | Test Accuracy |
|-------|---------|---------------------|---------------|
| Phase 1 | Kaggle | ~95% | ~90% |
| Phase 2 | YouTube | ~92% | ~88% |
| Phase 3 | Different Devices | ~85% | ~45% (device bias) |
| Phase 4 | Same Device | ~90% | ~87% (solved!) |

## How to Run
1. Install dependencies: `pip install tensorflow librosa numpy pandas matplotlib seaborn`
2. Open `final-project.ipynb` in Jupyter Notebook
3. Run cells sequentially to reproduce results

## Dataset Note
Datasets are not included in this repository due to size constraints. Dataset sources are documented in the notebook.

## Author
ECE 5831 - Pattern Recognition and Neural Networks
University of Michigan-Dearborn
2025
