🗣️ Scream Detection and Crime Prevention System

This project is designed to detect human screams in real-time using machine learning and audio processing. It can be integrated into surveillance systems or safety tools to automatically detect distress or danger.

---

## 📦 Dataset

To use this project, download the dataset from Kaggle:

🔗 [Human Screaming Detection Dataset](https://www.kaggle.com/datasets/whats2000/human-screaming-detection-dataset/data)

After downloading:
1. Extract it into a folder named `dataset/` inside the project root.
2. The folder should look like:

```

/dataset
├── scream\_01.wav
├── normal\_01.wav
└── ...

````

---

## 🧪 Feature Extraction

To convert audio files into usable features:

### 🔁 Option 1: Run the script
```bash
python extract_features.py
````

This will generate a `features.csv` file.

### ⏩ Option 2: Skip and use our file

You can directly use the pre-generated `features.csv` from this repository.

---

## 🤖 Model Training

To train the model:

### 🔁 Option 1: Run the training script

```bash
python train_model.py
```

This will save a model file like `scream_detector_model.pkl`.

### ⏩ Option 2: Use our pretrained model

You can directly use the `scream_detector_model.pkl` file provided in the repo.

---

## 🎧 Real-Time Detection

To test real-time detection with your microphone:

```bash
python real_time_detection.py
```

This script listens through your mic and detects if a scream occurs based on the trained model.

---

## 📁 Project Structure

```
scream-detection/
├── dataset/                      # (Not included in repo, download from Kaggle)
├── features.csv                  # Extracted features
├── extract_features.py           # Script to extract features from audio
├── train_model.py                # Script to train ML model
├── scream_detector_model.pkl     # Trained model file
├── real_time_detection.py        # Real-time mic-based detection
└── README.md
```

---

## ⚙️ Requirements

Install dependencies using:

```bash
pip install -r requirements.txt
```

Basic libraries used:

* `numpy`
* `pandas`
* `librosa`
* `scikit-learn`
* `sounddevice`
* `scipy`
* `joblib`

---

## 🙌 Acknowledgements

* Dataset by [Whats2000 on Kaggle](https://www.kaggle.com/datasets/whats2000/human-screaming-detection-dataset/data)

---

## 💡 Future Enhancements

* Alerting system with SMS or email
* Integration with smart home or security systems
* Noise filtering and multi-source audio separation

---

## 🛡️ Disclaimer

This tool is for educational and safety research purposes only.

```
