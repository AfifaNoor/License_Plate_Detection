License Plate Recognition

Overview
The License Plate Recognition project aims to identify and recognize vehicle license plates using two distinct datasets:

Vehicle Images: Contains 900 images of vehicles, annotated with bounding boxes around the license plates.
License Plate Images: Contains 900 images of license plates, annotated with the alphanumeric text inscribed on them.
The project's objectives are twofold:

Detect and locate license plates in vehicle images.
Recognize and decipher the alphanumeric text on these license plates.

Dataset
Training Set 1
Description: 900 images of vehicles, each containing a license plate.
Annotations: Bounding box coordinates (ymin, xmin, ymax, xmax) for each license plate.

Training Set 2
Description: 900 images of license plates.
Annotations: Alphanumeric text on each license plate.
Test Set
Description: 201 images of vehicles.
Task: Detect and recognize license plates and their characters.
Project Structure
bash

ProjectRoot/
│
├── data/
│   ├── license_plates_detection_train/      # Folder containing images with cars and their corresponding license plates for detection
│   ├── license_plates_recognition_train/    # Folder containing images of license plates for recognition
│   ├── test/                                # Folder containing test images
│   ├── Licplatesdetection_train.csv         # CSV file with bounding box annotations for detection
│   ├── Licplatesrecognition_train.csv       # CSV file with text annotations for recognition
│   ├── SampleSubmission.csv                 # CSV file for submission template
│
├── notebooks/
│   ├── License_Plate_Recognition.ipynb      # Jupyter Notebook with the complete code for the project
│
├── results/
│   ├── results_detection/                   # Folder containing detection results (images with drawn bounding boxes)
│   ├── results_recognition/                 # Folder containing recognition results (text files with recognized license plate characters)
│
├── requirements.txt                         # File containing the list of required packages and their versions
│
└── README.md                                # Project description and instructions (this file)
Installation
To run this project, you'll need the following Python packages. You can install them using pip:

bash
Copy code
pip install -r requirements.txt

Usage
Data Preparation
Download the datasets and place them in the data folder.
Ensure the Licplatesdetection_train.csv and Licplatesrecognition_train.csv files are in the data folder.

Training the Model
Open the Jupyter Notebook License_Plate_Recognition.ipynb.
Follow the instructions in the notebook to preprocess the data, build the models, and train them.

Evaluation
The notebook includes sections to evaluate the performance of the detection and recognition models.
Evaluation results will be saved in the results folder.

Results
Detection Results: Results with drawn bounding boxes on images will be saved in results/results_detection.
Recognition Results: Recognized characters and their accuracy will be saved in results/results_recognition.

.

