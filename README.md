# NYC Airbnb Room Type Predictor

A Machine Learning web application that predicts the Airbnb room type (Entire home/apt, Private room, Shared room) based on listing features in New York City.

## Overview

- **Machine Learning Pipeline**: Trained using Scikit-Learn with data preprocessing, categorical encoding, and classification pipeline saved as `Model_Pipeline.pkl`.
- **Backend API**: High-performance REST API built with **FastAPI** and **Pydantic** for input schema validation.
- **Frontend UI**: Interactive web interface with modern responsive design to enter listing features and view live predictions with probability scores.
- **Exploratory Data Analysis (EDA)**: Detailed Jupyter Notebook (`nyc_airbnb_room_type_classification.ipynb`) covering data cleaning, visualization, feature engineering, and model training.

## Tech Stack

- **Python 3**
- **FastAPI** & **Uvicorn**
- **Scikit-Learn**, **Pandas**, **Joblib**
- **Pydantic**
- **HTML5, CSS3, JavaScript**

## Project Structure

```
├── main.py                                  # FastAPI application & prediction endpoints
├── Model_Pipeline.pkl                       # Trained Scikit-Learn ML pipeline
├── nyc_airbnb_room_type_classification.ipynb # Notebook with EDA & model training
├── index.html                               # Frontend UI
├── style.css                                # Frontend styling
├── script.js                                # Frontend logic & API interaction
├── the_build_line_guide.html                # Project guide & reference
├── requirements.txt                         # Python dependencies
└── runtime.txt                              # Python runtime specification
```

## Getting Started

### 1. Setup Virtual Environment & Install Dependencies

```bash
python -m venv venv
# On Windows:
venv\Scripts\activate
# On Linux/macOS:
source venv/bin/activate

pip install -r requirements.txt
```

### 2. Run the FastAPI Server

```bash
uvicorn main:app --reload
```
The API will be available at `http://127.0.0.1:8000`. Interactive API documentation is available at `http://127.0.0.1:8000/docs`.

### 3. Open the Frontend

Open `index.html` in your browser to interact with the prediction UI.
