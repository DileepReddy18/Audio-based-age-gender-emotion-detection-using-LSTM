
# Audio-Based Emotion, Age, and Gender Recognition Using Deep Learning

This project focuses on building an AI-powered system to classify **gender**, **age**, and **emotion** from audio files using deep learning and machine learning techniques. The system leverages advanced audio processing libraries like `librosa` and models such as LSTM, Random Forest, and SVM to achieve accurate predictions.

---

## Table of Contents

1. [Project Overview](#project-overview)
2. [Datasets](#datasets)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Screenshots](#screenshots)
6. [Contributing](#contributing)
7. [License](#license)

---

## Project Overview

The goal of this project is to analyze audio data and predict:
- **Gender**: Male or Female
- **Age**: Age group (e.g., teens, twenties, etc.)
- **Emotion**: Emotional state (e.g., happy, sad, angry, etc.)

We use:
- **Deep Learning**: LSTM for gender classification.
- **Machine Learning**: Random Forest for age classification and SVM for emotion classification.

---

## Datasets

The project relies on two publicly available datasets:

### 1. **CREMA-D Dataset**
- **Description**: A dataset for emotion recognition containing audio recordings of actors expressing various emotions.
- **Download Link**: [CREMA-D Dataset](https://github.com/CheyneyComputerScience/CREMA-D)

### 2. **Mozilla Common Voice Dataset**
- **Description**: A large open-source dataset of human voices contributed by volunteers worldwide. It contains metadata such as gender and age annotations.
- **Download Link**: [Mozilla Common Voice Dataset](https://commonvoice.mozilla.org/en/datasets)

---

## Installation

### Prerequisites
- Python 3.9+
- Libraries: `numpy`, `pandas`, `librosa`, `tensorflow`, `scikit-learn`, `joblib`, `flask` (or another web framework for the frontend).

### Steps to Set Up

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/audio-based-age-gender-emotion.git
   cd audio-based-age-gender-emotion
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Download the datasets:
   - Download the [CREMA-D Dataset](https://github.com/CheyneyComputerScience/CREMA-D) and place it in the `data/CREMA-D Dataset` directory.
   - Download the [Mozilla Common Voice Dataset](https://commonvoice.mozilla.org/en/datasets) and extract the `clips` folder and `validated.tsv` file into the `data/Mozilla Common Voice Dataset` directory.

4. Train the models:
   ```bash
   python src/train_models.py
   ```

5. Run the application:
   ```bash
   python app.py  # Replace with your web app script name
   ```

---

## Usage

1. **Upload or Record Audio**:
   - Use the web interface to upload an audio file or record one directly using your microphone.

2. **View Predictions**:
   - The system will process the audio and display predictions for:
     - Gender (Male/Female)
     - Age Group (e.g., teens, twenties, etc.)
     - Emotion (e.g., happy, sad, angry, etc.)

---

## Screenshots

### 1. Home Page
![Home Page](https://github.com/DileepReddy18/Audio-based-age-gender-emotion-detection-using-LSTM/blob/7313ff25f3f48d6b7b7d8f9e2b701bb6ced7b719/Screenshot%202025-04-23%20162246.png)  
*The main interface where users can upload or record audio.*

### 2. Results Page
![Results Page](https://github.com/DileepReddy18/Audio-based-age-gender-emotion-detection-using-LSTM/blob/7313ff25f3f48d6b7b7d8f9e2b701bb6ced7b719/Screenshot%202025-04-25%20101305.png)  
*Displays the predicted gender, age, and emotion.*

---

## Contributing

We welcome contributions to improve this project! To contribute:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeatureName`).
3. Commit your changes (`git commit -m "Add YourFeatureName"`).
4. Push to the branch (`git push origin feature/YourFeatureName`).
5. Open a pull request.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Acknowledgments

- Thanks to the creators of the [CREMA-D Dataset](https://github.com/CheyneyComputerScience/CREMA-D) and [Mozilla Common Voice Dataset](https://commonvoice.mozilla.org/en/datasets) for providing open-source datasets.
- Special thanks to libraries like `librosa`, `tensorflow`, and `scikit-learn` for enabling audio processing and machine learning.

---
