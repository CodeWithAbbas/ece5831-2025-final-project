# ECE 5831 - Speaker Recognition Final Project

## Overview
A deep learning speaker recognition system using LSTM neural networks with MFCC features. This project explores model performance across different datasets and discovers critical device bias issues in audio machine learning models.

## Project Links

### Presentation & Documentation
- **Presentation Video**: https://drive.google.com/file/d/18FurAJvFekTY0bxIUZxCxioVUDz2XvLo/view?usp=drive_link
- **Presentation Slides**: https://drive.google.com/drive/folders/1EE2xPEZ3LIH0Al7JThV6rQaEalsaASIT?usp=sharing
- **Project Report**: https://drive.google.com/file/d/1oqJ02mYSLgNO75fYVXRR4euNhWvZzv3I/view?usp=drive_link

### Resources
- **Dataset**: https://drive.google.com/drive/folders/1_zFiw8QxHIFUgCKe5_8ioB5KZ788SJvI?usp=drive_link
- **Demo Video**: https://youtu.be/KdgDX2zgr6o

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
- `final-project.ipynb` - Complete project notebook with executed cells
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
1. Download the dataset from the Google Drive link above
2. Install dependencies: `pip install tensorflow librosa numpy pandas matplotlib seaborn`
3. Open `final-project.ipynb` in Jupyter Notebook
4. Update dataset paths in the notebook to point to your downloaded dataset location
5. Run cells sequentially to reproduce results

## Dataset Information
The complete dataset is available on Google Drive (link above). It includes:
- Kaggle speaker recognition dataset
- YouTube public figures audio samples
- Custom device recordings for bias analysis

## Team Members & Contributions
**Abbas Ali, Shravya Kumbham, Hesham Aldahbali**

All team members contributed equally to this project, with shared responsibilities across all phases including:
- Literature review and research
- Data collection and preprocessing
- Model development and implementation
- Experimentation and debugging (including the critical device bias discovery)
- Analysis and documentation
- Presentation and reporting

This project represents a collaborative effort where each team member actively participated in all aspects of the work.

---

ECE 5831 - Pattern Recognition and Neural Networks
University of Michigan-Dearborn
December 2025
