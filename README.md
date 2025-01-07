# APK Obfuscation Detector

This program is an interactive tool built in Python for detecting obfuscation in Android APK files. It uses machine learning models to analyze APK features such as file size, DEX count, and permissions to predict whether an APK is obfuscated.

# DEMO VIDEO

https://github.com/user-attachments/assets/0e42e5e7-b7d6-4b6a-a123-9305e696644b


## 🛠️ Features
- **APK Upload**: Upload APK files via an interactive widget in Jupyter Notebook.
- **Feature Extraction**: Extracts file size, DEX count, and permissions from the APK using `androguard`.
- **Machine Learning Analysis**: Predicts obfuscation using a pre-trained Random Forest model.
- **Detailed Results**: Provides prediction status, confidence levels, and detected permissions in a user-friendly output.

## 🚀 How It Works
1. Upload the APK file using the provided interface.
2. The program extracts relevant features from the APK.
3. Features are encoded and passed to the Random Forest model for prediction.
4. Results are displayed, including:
   - Obfuscation status
   - Prediction confidence
   - APK details (file size, DEX count, permissions)

## 🧰 Prerequisites
- Python 3.7 or higher
- Jupyter Notebook
- Required Python libraries:
  - `androguard`
  - `pandas`
  - `pickle`
  - `joblib`
  - `ipywidgets`

## 📂 File Structure
- **`apk_obfuscation_detector.py`**: Main program file.
- **`multi_label_binarizer.pkl`**: Pre-trained MultiLabelBinarizer for encoding permissions.
- **`random_forest_model.pkl`**: Pre-trained Random Forest model for prediction.

  ## 📈 Methodology
1. Feature Extraction: Extract key features using androguard.
2. Data Preparation: Encode permissions using the MultiLabelBinarizer.
3. Prediction: Use the Random Forest model to classify APKs.
4. Results Display: Present results in a readable, interactive format.

## 🖥️ Usage
Launch Jupyter Notebook:
```bash
jupyter notebook

Install dependencies with:
```bash
pip install androguard pandas joblib ipywidgets




