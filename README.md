# ML-OPS
The MLOps (Machine Learning Operations) Pipeline automates the end-to-end lifecycle of a machine learning model, from training to deployment and monitoring. This ensures that models are scalable, reproducible, and continuously improved.

Pipeline Breakdown:
1. Model Training & Experiment Tracking (MLflow)
Loads a dataset and trains a Random Forest model.
Uses MLflow to track hyperparameters (n_estimators), model performance (accuracy), and store model versions.
Ensures reproducibility of experiments for future comparisons.
2. Model Packaging & Deployment (Flask & Docker)
Saves the trained model (model.pkl) for later inference.
Builds a Flask API that takes input features and returns predictions.
Packages the API and model inside a Docker container for deployment in any environment.
3. CI/CD Automation (GitHub Actions)
Automates the deployment process every time new code is pushed.
Builds and runs the Docker container to serve predictions.
Ensures continuous integration and delivery without manual intervention.
Key Technologies Used:
* MLflow – Experiment tracking and model versioning
* Docker & Kubernetes – Containerization and orchestration
* Flask API – Model serving as a REST endpoint
* CI/CD (GitHub Actions) – Automating deployments
* Cloud Integration (AWS/GCP) – Deploying models at scale

This MLOps pipeline ensures efficient, scalable, and automated deployment of machine learning models in production.
