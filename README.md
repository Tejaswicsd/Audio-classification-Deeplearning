# Audio-classification-Deeplearning
# Urban Sound Classification using Deep Learning  

## Project Overview  
This project classifies **urban sound events** (such as sirens, car horns, drilling, etc.) using **deep learning models** trained on the [UrbanSound8K dataset](https://urbansounddataset.weebly.com/urbansound8k.html).  
Achieved **89% accuracy** by extracting **MFCC features** and training a neural network with TensorFlow & Keras.  

---

## Tech Stack  
- **Language:** Python  
- **Libraries:** TensorFlow, Keras, NumPy, Pandas, Librosa, Scikit-learn, Matplotlib  
- **Dataset:** UrbanSound8K  

---

##  Features  
- End-to-end ML pipeline (preprocessing → training → evaluation → prediction)  
- **Feature Extraction:** MFCCs (Mel-Frequency Cepstral Coefficients)  
- **Model:** Deep Neural Network (CNN / LSTM variations possible)  
- **Accuracy:** ~89% on test data  
- Audio visualization (waveforms & spectrograms)  

---

## Project Structure  
```bash
├── data/                  # UrbanSound8K dataset
├── notebooks/             # Jupyter notebooks for experiments
├── models/                # Saved models (.h5 files)
├── src/                   # Source code
│   ├── preprocess.py      # Data cleaning & feature extraction
│   ├── train.py           # Model training script
│   ├── evaluate.py        # Testing & evaluation
│   └── predict.py         # Predict on new audio file
├── requirements.txt       # Dependencies
└── README.md              # Project documentation
 Installation & Setup

Clone this repository:
git clone https://github.com/Tejaswicsd/Audio-classification-Deeplearning.git
cd Audio-classification-Deeplearning
Create a virtual environment & install dependencies:
pip install -r requirements.txt
Place the UrbanSound8K dataset inside the data/ folder.
Usage

Training the Model:
python src/train.py
Evaluating the Model:
python src/evaluate.py
Predicting a New Audio File:
python src/predict.py --file sample.wav
Results

Achieved ~89% accuracy on the UrbanSound8K dataset.

MFCCs proved highly effective for urban sound recognition.
Future Enhancements

Experiment with CNN + LSTM hybrid models for better temporal feature extraction.

Deploy as a Flask / FastAPI web app for real-time audio classification.

Optimize model for edge devices.
 Author

Tejaswi Guttula
