# KidneySense: Kidney Disease Classification System - Still at Testing 

## Overview

KidneySense is an end-to-end Deep Learning and MLOps project designed to automatically classify kidney diseases from medical images. The project leverages Convolutional Neural Networks (CNNs) for accurate disease detection while incorporating industry-standard MLOps practices such as experiment tracking, data versioning, pipeline orchestration, containerization, and cloud deployment.

The system is built with a modular architecture to ensure scalability, reproducibility, and maintainability throughout the machine learning lifecycle.

## Key Features

* Deep Learning-based Kidney Disease Classification
* Modular and Production-Ready Project Structure
* Experiment Tracking using MLflow
* Data and Model Versioning using DVC
* Automated Training Pipelines
* Docker Containerization
* CI/CD Automation with GitHub Actions
* AWS Deployment Support
* Interactive Web Application for Predictions

## Tech Stack

### Machine Learning

* Python
* TensorFlow / Keras
* NumPy
* Pandas
* Scikit-learn

### MLOps

* MLflow
* DVC
* GitHub Actions
* Docker

### Cloud & Deployment

* AWS EC2
* AWS ECR

## Project Architecture

The project follows a complete MLOps workflow:

1. Data Ingestion
2. Data Validation
3. Data Transformation
4. Model Training
5. Model Evaluation
6. Experiment Tracking
7. Pipeline Orchestration
8. Model Deployment

## Workflows

1. Update config.yaml
2. Update params.yaml
3. Update entity configuration
4. Update Configuration Manager
5. Update Components
6. Update Pipelines
7. Update main.py
8. Update dvc.yaml
9. Run Training Pipeline
10. Launch Application

## Installation

### Clone Repository

```bash
git clone https://github.com/<your-username>/KidneySense.git
cd KidneySense
```

### Create Environment

```bash
conda create -n kidneysense python=3.8 -y
conda activate kidneysense
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Run Application

```bash
python app.py
```

Open the generated localhost URL in your browser.

## MLflow

Launch MLflow UI:

```bash
mlflow ui
```

MLflow helps:

* Track experiments
* Compare model performance
* Log parameters and metrics
* Manage model versions

## DVC

Useful Commands:

```bash
dvc init
dvc repro
dvc dag
```

DVC helps:

* Version datasets
* Track model artifacts
* Reproduce experiments
* Build ML pipelines

## Docker Deployment

Build Docker Image:

```bash
docker build -t kidneysense .
```

Run Container:

```bash
docker run -p 8080:8080 kidneysense
```

## AWS CI/CD Deployment

The project supports automated deployment using:

* AWS EC2
* AWS ECR
* GitHub Actions
* Docker Containers

Deployment Workflow:

1. Build Docker Image
2. Push Image to AWS ECR
3. Pull Image on EC2
4. Deploy Updated Application
5. Monitor Deployment

## Future Enhancements

* Explainable AI using Grad-CAM
* Multi-Class Kidney Disease Detection
* PDF Medical Report Generation
* Real-Time Clinical Dashboard
* Integration with Electronic Health Records
* XAI reports
  thanks to krish nayak sir for bringing in with the understanding of MLOPS
