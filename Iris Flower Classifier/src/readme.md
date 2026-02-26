🌸 Iris Flower Species Classifier

An end-to-end Machine Learning project that classifies iris flowers into three species using a production-style architecture. This project demonstrates an MLOps-lite pipeline, integrating model training, API deployment, and frontend interaction in a cleanly structured and scalable way.

📌 Project Objectives

Classification: Accurately predict iris flower species — Setosa, Versicolor, or Virginica.

Architecture Best Practices: Maintain separation between:

Machine Learning logic (training & inference)

Backend API layer

Frontend user interface

Professional Tooling: Use industry-standard Python tools for real-world workflow simulation.

🛠️ Technology Stack

Machine Learning: Scikit-learn

Model Persistence: Joblib

Backend API: Flask

Frontend UI: Streamlit

📂 Project Structure
iris-classifier/
├── src/
│   ├── __init__.py              # Python package marker
│   ├── model_trainer.py         # Data ingestion, training & serialization
│   ├── prediction_api.py        # Flask API for real-time predictions
│   └── web_app.py               # Streamlit frontend interface
├── models/
│   ├── iris_knn_model.pkl       # Serialized trained model
│   └── iris_target_names.pkl    # Label-to-species mapping
├── README.md                    # Project documentation
├── requirements.txt             # Python dependencies
└── run_project.sh               # Optional automation script

The structure ensures clean separation of concerns, making the project scalable and production-ready.

🚀 Getting Started
1️⃣ Prerequisites

Python 3.x

pip package manager

2️⃣ Setup & Installation

From the project root directory:

pip install -r requirements.txt
mkdir models
3️⃣ Execution Workflow

The application requires three steps. Run each in a separate terminal window.

🔹 Step A: Train the Model

Trains the K-Nearest Neighbors model and saves artifacts.

python src/model_trainer.py
🔹 Step B: Start the Backend API

Launches the Flask server on Port 5000.

python src/prediction_api.py

Keep this terminal running.

🔹 Step C: Launch the Frontend UI

Starts the Streamlit interface.

streamlit run src/web_app.py

The web app will open in your browser and communicate with the running API in real time.

🤖 Model Details
📊 Dataset

The model is trained on the classic Iris dataset containing 150 samples across three species:

Iris Setosa

Iris Versicolor

Iris Virginica

🧠 Algorithm

The classifier uses the K-Nearest Neighbors (KNN) algorithm with:

K = 3

KNN predicts a flower’s species based on the majority class among its three closest neighbors in feature space.

📥 Input Features

The model uses four numerical features:

Sepal Length (cm)

Sepal Width (cm)

Petal Length (cm)

Petal Width (cm)

🛑 Shutting Down

To properly stop the application:

Close the Streamlit browser tab.

In the Flask API terminal, press:

Ctrl + C
🎯 Key Highlights

Clean ML → API → UI separation

Real-time prediction workflow

Model serialization & deployment simulation

Scalable project structure

Beginner-friendly yet industry-aligned

📌 Ideal For

Machine Learning portfolio projects

Demonstrating backend + frontend ML integration

Learning deployment fundamentals

Showcasing production-style Python architecture
