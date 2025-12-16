# ECE 5831 - Speaker Recognition Final Project

## Overview
A deep learning speaker recognition system using LSTM neural networks with MFCC features. This project explores model performance across different datasets and discovers critical device bias issues in audio machine learning models.

## Project Links

### Presentation & Documentation
- **Presentation Video**: [Link to YouTube Video]
- **Presentation Slides**: [Link to Google Drive - Presentation]
- **Project Report**: [Link to Google Drive - Report]

### Resources
- **Dataset**: [Link to Google Drive - Dataset]
- **Demo Video**: [Link to YouTube Demo]
- **YouTube Channel**: [Link to Channel]

### Google Drive Folder
- **Complete Project Files**: [Link to ece5831-2025-final-project folder]
  - Includes: dataset, presentation, and report subdirectories

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

## Author
ECE 5831 - Pattern Recognition and Neural Networks
University of Michigan-Dearborn
2025
