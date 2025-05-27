# ML Mini Project – Audio Classification

This repo contains two machine learning mini-projects developed as part of the *Principles of Machine Learning* module during my MSc in Big Data Science at Queen Mary University of London.

The task was to classify audio recordings — created by students whistling or humming — using classical ML techniques. The dataset was provided by the course lecturer and consisted of `.wav` files with labeled content.

## Project Structure

- `miniproject_basic.ipynb`  
  Binary classification: humming vs. whistling

- `miniproject_advanced.ipynb`  
  Multiclass classification: classify one of three melodies (Harry Potter, Star Wars, Pink Panther)

## Technologies & Libraries

- Python, NumPy, Pandas, Matplotlib
- `librosa` for audio feature extraction
- `scikit-learn` for ML models and evaluation
- `xgboost` for gradient boosting
- Jupyter Notebooks

## ML Models Used

- Logistic Regression
- Support Vector Machine
- Naive Bayes
- Multilayer Perceptron (MLP)
- XGBoost

Each model was evaluated using accuracy, confusion matrix, Cohen's Kappa, and Matthews Correlation Coefficient.

## Audio Features Extracted

- Mel-frequency cepstral coefficients (MFCCs)
- Spectral bandwidth
- Tempo estimation

Features were normalized using MinMaxScaler.

## How to Run

This project was developed and tested using Google Colab.

To run it:
1. Open either `miniproject_basic.ipynb` or `miniproject_advanced.ipynb` in Colab
2. Ensure the required packages listed in `requirements.txt` are available in your runtime

> **Note**: The original dataset links provided in the notebooks are no longer active. To run the project, you will need to supply your own audio data and adjust the file paths accordingly.

> **Note for non-Colab users**:  
> This project assumes a Google Colab environment and uses Google Drive paths (e.g., `/content/drive/MyDrive/...`).  
> To run it locally, you’ll need to:  
> - Remove or comment out `drive.mount()`  
> - Replace all `/content/drive/...` paths with your local equivalents

## Dependencies

You can install everything using:

```bash
pip install -r requirements.txt
```
