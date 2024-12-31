# Machine Failure Predictor

## Overview

The `Machine Failure Predictor` is a web application designed to enable predictive maintenance for industrial equipment. Leveraging machine learning techniques, this application predicts whether equipment will fail and identifies the type of failure based on key process parameters. The system aims to improve operational efficiency by minimizing unplanned downtime and reducing repair costs.

The project utilizes a synthetic dataset of process parameters, including air and process temperatures, rotational speed, torque, and tool wear. The application integrates a machine learning backend with an intuitive web interface, making it accessible to users without extensive technical expertise.

---

## Features

### Core Functionalities
- **Failure Prediction**: Predicts whether the equipment will fail based on provided process parameters.
- **Failure Classification**: Identifies the type of failure (if any) using multi-class classification.
- **Model Insights**: Allows users to compare performance metrics (e.g., precision, recall, F1 score) of different models.
- **Data Visualization**: Provides interactive visualizations to help users understand trends and equipment behavior.

### Technical Highlights
- **Backend**: Built with FastAPI for high-performance API handling.
- **Frontend**: Interactive and user-friendly interface developed using Streamlit.
- **Deployment**: Packaged and deployed using Docker and hosted on DigitalOcean droplets for scalability and reliability.
- **MLOps Integration**: End-to-end automation using a CI/CD pipeline powered by GitHub Actions.

---

## Motivation

Predictive maintenance is critical for industrial operations to ensure seamless performance and cost-effectiveness. The traditional reactive maintenance approach often leads to extended downtimes and inflated repair costs. By predicting failures before they occur, businesses can schedule timely maintenance, leading to:
- Reduced operational interruptions.
- Lower maintenance costs.
- Increased equipment lifespan.
- Enhanced safety and reliability.

---

## Success Metrics

The success of the application is measured by:
1. **Model Performance**: High precision, recall, and F1 score across binary and multi-class classification models.
2. **User Experience**: A responsive, intuitive, and secure web interface.
3. **Operational Impact**: Significant reduction in unplanned downtime and maintenance costs.

---

## System Requirements and Constraints

### Functional Requirements
- Accept process parameters as input and return predictions.
- Display model performance metrics for transparency.
- Provide tools for visualizing data trends and model insights.

### Non-functional Requirements
- High accuracy and reliability of predictions.
- Secure handling of user data and inputs.
- Optimized for low-cost deployment and high responsiveness.

### Constraints
- Built with **FastAPI** and **Streamlit**.
- Deployed using **Docker** containers on **DigitalOcean**.
- Limited to synthetic dataset use and predictive analytics.

### Out-of-Scope
- Integration with external applications or live data sources.
- Detailed diagnostic capabilities for specific equipment components.

---

## Dataset

The application uses a synthetic dataset comprising over 50,000 records and 14 features:
- **Inputs**: Air temperature, process temperature, rotational speed, torque, tool wear.
- **Target Variables**: 
  - Binary label indicating failure (yes/no).
  - Multi-class label specifying the failure type (e.g., heat dissipation, power failure, mechanical vibration).

Preprocessing steps include missing value imputation, feature scaling, and encoding of categorical variables.

---

## Methodology

### Machine Learning Techniques
1. **Data Preprocessing**: Cleaning and transforming raw data for model input.
2. **Feature Engineering**: Selecting the most impactful features for prediction.
3. **Model Training**: Training binary and multi-class classification models.
4. **Hyperparameter Tuning**: Optimizing models for maximum accuracy.
5. **Model Evaluation**: Assessing performance using precision, recall, F1 score, and other metrics.

### Pipeline Workflow
1. **Data Preprocessing**: Data cleaning and preparation.
2. **Model Training**: Training multiple machine learning models.
3. **Evaluation**: Selecting the best-performing model.
4. **Deployment**: Packaging the application using Docker.
5. **Integration**: Hosting on DigitalOcean and automating updates with CI/CD pipelines.

---

## Architecture

The application architecture consists of the following components:
- **Frontend**: Streamlit-based interface for user interaction.
- **Backend**: FastAPI server managing API requests and model inference.
- **Machine Learning Models**: Binary and multi-class classifiers.
- **Containerization**: Dockerized application components for consistent deployment.
- **Cloud Hosting**: Deployed on DigitalOcean droplets for scalability and reliability.
- **CI/CD Pipeline**: Automated testing and deployment using GitHub Actions.

---

## Deployment

### Tools and Technologies
- **Programming Languages**: Python.
- **Frameworks**: FastAPI, Streamlit.
- **Machine Learning Libraries**: Scikit-learn, Pandas, NumPy.
- **Visualization**: Matplotlib, Seaborn, Plotly.
- **Containerization**: Docker.
- **Hosting**: DigitalOcean.
- **CI/CD**: GitHub Actions.

---

## How to Use

1. Clone the repository:
   ```bash
   git clone https://github.com/themihirmathur/Machine-Failure-Predictor.git
   ```
2. Navigate to the project directory:
   ```bash
   cd Machine-Failure-Predictor
   ```
3. Build Docker containers:
   ```bash
   docker-compose up --build
   ```
4. Access the application in your browser at:
   ```
   http://<your-digitalocean-droplet-ip>:8501
   ```

---

## Conclusion

The **Machine Failure Predictor** serves as a practical solution for predictive maintenance, empowering users to minimize downtime and optimize operations. By leveraging advanced machine learning techniques, the application offers actionable insights to maintain equipment health effectively. Future enhancements may include integration with real-time data sources and expanded diagnostic capabilities.

For more details or to contribute, visit the [GitHub Repository](https://github.com/themihirmathur/Machine-Failure-Predictor.git).
