
# AI-Assisted-ECG-Diagnosis

## Overview
AI-Assisted-ECG-Diagnosis is a machine learning and deep learning project aimed at diagnosing heart conditions from ECG data using artificial intelligence. This project leverages raw ECG signals, biological data such as age and sex, and applies various models to classify ECG signals into diagnostic categories.

## Project Status
This project is still under development and is not finalized yet. The current notebook includes data loading, preprocessing, feature extraction, and some initial models. Future iterations will improve model accuracy and explore additional techniques like deep learning.

## Features
- **ECG Signal Processing**: Uses raw ECG signal data, along with biological features such as age and sex, to predict diagnostic results.
- **Multi-Class Classification**: The system is designed to classify ECG signals into multiple diagnostic classes.
- **Deep Learning**: Implements models like LSTM and CNN for analyzing ECG signals.
- **Data Preprocessing**: Includes data cleaning, feature extraction, and handling imbalanced data with techniques like SMOTE.

## Requirements
- Python 3.x
- Libraries:
  - pandas
  - numpy
  - sklearn
  - tensorflow
  - imbalanced-learn
  - xgboost
  - wfdb (for ECG data processing)

## Getting Started
1. Clone or download the repository.
2. Install the required libraries by running:
   ```bash
   pip install -r requirements.txt
   ```
3. Load the dataset (ECG signals, annotations, etc.) into the project directory.
4. Follow the instructions in the Jupyter notebook to run the code.

## Usage
Run the provided Jupyter notebook to:
- Load and preprocess ECG signal data.
- Train machine learning and deep learning models.
- Evaluate model performance with various metrics.

## Future Work
- Improve the deep learning models for better classification accuracy.
- Experiment with other types of machine learning models.
- Integrate more sophisticated signal processing techniques.
- Expand the dataset and include more diagnostic labels.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
