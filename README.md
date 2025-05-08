# Crop Disease Detection using YOLOv11

This repository contains the source code for training, validation, and deployment of a crop disease classification system using the YOLOv11 architecture on the augmented PlantVillage dataset.

---

## Repository Structure

- `ModelTrainingAndValidation.ipynb`  
  Jupyter Notebook containing the complete training and validation pipeline.

- `runs/`  
  Directory containing results, logs, and model checkpoints from different training runs.

- `WebApplication/`  
  Front-end web application to test predictions using the trained model.

---

## Training and Validation

The model is trained on **38 classes** of healthy and diseased plants using the **augmented PlantVillage** dataset. All training logic is provided in:

```bash
ModelTrainingAndValidation.ipynb
```

## Running the Web Application

To start the web-based interface for disease prediction:

Clone the repository

```bash
git clone https://github.com/nitinsomu/CropDiseaseDetectionYOLOv11.git
cd CropDiseaseDetectionYOLOv11/WebApplication
```

Create and activate a virtual environment

```bash
python -m venv venv
# On Windows
venv\Scripts\activate
# On macOS/Linux
source venv/bin/activate
```

Install the required dependencies

```bash
pip install -r requirements.txt
```

Run the application

```bash
python app.py
```

The app will launch locally and allow users to upload images for classification at http://127.0.0.1:10000.

## Pretrained Model Reference

This project leverages the YOLOv11 classification model - YOLO11m-cls. For detailed architecture and functionality, refer to the Ultralytics Classification Docs (https://docs.ultralytics.com/tasks/classify/).
