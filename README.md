# **Chest Cancer Classification Project with MLOps**

This project showcases an **end-to-end deep learning implementation** for classifying chest cancer using CT scan images. Leveraging **MLflow** and **DVC**, this project incorporates MLOps principles, focusing on efficient experiment tracking, modular pipeline design, and deployment-ready solutions.

---

## **Features**

- **Comprehensive Workflow**:
  - Modular implementation of deep learning pipelines.
  - Utilizes MLflow for experiment tracking and model registration.
  - Tracks and optimizes data pipelines with DVC.

- **Scalable Framework**:
  - Seamless integration of MLflow with local and remote servers.
  - CICD-based deployments using Docker and cloud platforms.

- **User-Friendly Interface**:
  - Deployable web app for cancer classification.
  - Real-time predictions from CT scan images.

---

## **Tech Stack**

- **Languages**: Python
- **Libraries**: TensorFlow, Keras, MLflow, DVC
- **Deployment**: Docker, AWS, Azure
- **Frontend**: HTML, CSS (basic)
- **Version Control**: GitHub

---

## **Directory Structure**

```bash
├── app
│   ├── api
│   ├── pipeline
│   ├── templates
│   ├── utils
├── data
│   ├── raw
│   └── processed
├── experiments
│   └── MLflow runs and metadata
├── docker
├── models
├── notebooks
│   └── experiment_notebooks
└── requirements.txt
```

---

## **Getting Started**

### **Prerequisites**

1. **Python**: Install Python 3.8 or later.
2. **MLflow**: Set up MLflow locally or on a remote server like DagsHub or AWS.
3. **DVC**: Install DVC for data versioning.
4. **Docker**: Required for deployment.
5. **Cloud Accounts**: AWS and Azure credentials for deployment.

### **Installation**

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/chest-cancer-classification.git
   cd chest-cancer-classification
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Set up MLflow tracking URI:
   - For local: `http://localhost:5000`
   - For remote: Configure with your cloud-based URI.

---

## **How It Works**

### **Pipeline Overview**

1. **Data Ingestion**:
   - Raw CT scan images are processed into labeled datasets.
   - Metadata is managed using DVC.

2. **Preprocessing**:
   - Data augmentation techniques applied to normalize and enhance images.

3. **Training and Experimentation**:
   - Model training using TensorFlow with hyperparameter tuning.
   - MLflow tracks all experiment parameters, metrics, and artifacts.

4. **Deployment**:
   - Web application built to accept images and provide predictions.
   - Dockerized app deployed on AWS or Azure using CICD pipelines.

---

## **Project Highlights**

- **MLflow Experiment Tracking**:
  - Automatic logging of parameters, metrics, and models.
  - Supports both local and cloud deployments.

- **DVC Integration**:
  - Tracks dataset versions and ensures data consistency.

- **Web Interface**:
  - Intuitive image uploader to classify chest cancer from CT scans.
  - Predicts cancer types such as Adenocarcinoma.

---

## **Example Usage**

- **Run MLflow Server**:

  ```bash
  mlflow ui
  ```

- **Execute Training Pipeline**:

  ```bash
  python app/api/train.py --config config/train_config.yaml
  ```

- **Launch Application**:

  ```bash
  docker-compose up
  ```

---

## **Future Enhancements**

- Expand dataset for better accuracy.
- Improve web app UI using modern frameworks.
- Automate pipeline with more MLOps tools.

---

## **Contributing**

We welcome contributions! Please fork the repository and submit a pull request.

---

## **License**

MIT License - See [LICENSE](./LICENSE) for details.

---
