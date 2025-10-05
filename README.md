# Exoplanet Predictor Web App

This project contains two main files:  
- `train_model.py` — used to train a machine learning model on exoplanet data  
- `app2.py` — a Streamlit web app that uses the trained model to predict exoplanet status

## Getting Started

Follow these steps to set up and run the project from scratch, even as a beginner.

### 1. Install Python

Ensure that Python 3.8 or newer is installed. Download it from [python.org](https://www.python.org/) if needed.

### 2. Create a Virtual Environment

Open a terminal/command prompt in the project folder and run:
```sh
python -m venv venv
```
This creates a folder named `venv` containing a separate Python environment.

Activate your virtual environment:
- On Windows:
    ```sh
    venv\Scriptsctivate
    ```
- On macOS/Linux:
    ```sh
    source venv/bin/activate
    ```

### 3. Install Dependencies

First, upgrade pip:
```sh
pip install --upgrade pip
```

Then install the required packages:
```sh
pip install -r requirements.txt
```

### 4. Train the Model

Provide your dataset (for example, named `a.csv`) and run:
```sh
python train_model.py
```
This creates `model.joblib` and `scaler.joblib` which are needed for the web app.

### 5. Launch the Web App

Start the Streamlit app:
```sh
streamlit run app2.py
```
This will open a web browser window with the predictor interface.

### 6. Using the App

- Input required feature values as prompted.
- Click "Predict Exoplanet Status" to get a result and prediction confidence.

### Notes

- If you see `"Model files not found"` in the app, ensure `train_model.py` has been run and `model.joblib`/`scaler.joblib` exist in the same folder.
- A working internet connection may be needed for some Streamlit features (e.g., backgrounds or images).
- For dataset requirements, check the required columns/features used in the code.

---

These instructions make it easy for anyone, including beginners, to run and experiment with your project.
