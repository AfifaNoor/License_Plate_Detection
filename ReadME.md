# License Plate Recognition

## Overview

The License Plate Recognition project is designed to detect and recognize vehicle license plates using two distinct datasets:

1. **Vehicle Images**: Contains 900 images of vehicles, each annotated with bounding boxes around the license plates.
2. **License Plate Images**: Contains 900 images of license plates, annotated with the alphanumeric text on them.

### Project Objectives:

1. **License Plate Detection**: Detect and locate license plates in vehicle images.
2. **License Plate Recognition**: Recognize and decipher the alphanumeric text on these license plates.

## Dataset

### Training Set 1 (Detection)

- **Description**: 900 images of vehicles, each containing a license plate.
- **Annotations**: Bounding box coordinates (`ymin`, `xmin`, `ymax`, `xmax`) for each license plate.

### Training Set 2 (Recognition)

- **Description**: 900 images of license plates.
- **Annotations**: Alphanumeric text on each license plate.

### Test Set

- **Description**: 201 images of vehicles.
- **Task**: Detect and recognize license plates and the characters on them.

## Project Structure

```bash
ProjectRoot/
│
├── data/
│   ├── license_plates_detection_train/      # Folder containing vehicle images for detection
│   ├── license_plates_recognition_train/    # Folder containing license plate images for recognition
│   ├── test/                                # Folder containing test images
│   ├── Licplatesdetection_train.csv         # CSV file with bounding box annotations for detection
│   ├── Licplatesrecognition_train.csv       # CSV file with text annotations for recognition
│   ├── SampleSubmission.csv                 # CSV file for submission template
│
├── notebooks/
│   ├── License_Plate_Recognition.ipynb      # Jupyter Notebook with the complete code for the project
│
├── results/
│   ├── results_detection/                   # Folder containing detection results (images with bounding boxes)
│   ├── results_recognition/                 # Folder containing recognition results (recognized text)
│
├── requirements.txt                         # List of required packages and their versions
│
└── README.md                                # Project description and instructions (this file)
```

## Installation

To run this project, you’ll need the required Python packages. You can install them using:

```bash
pip install -r requirements.txt
```

## Usage

### Data Preparation

1. Download the datasets and place them in the `data` folder.
2. Ensure that `Licplatesdetection_train.csv` and `Licplatesrecognition_train.csv` are in the `data` folder.

### Training the Model

1. Open the Jupyter Notebook `License_Plate_Recognition.ipynb`.
2. Follow the instructions in the notebook to preprocess the data, build the models, and train them.

### Evaluation

- The notebook includes sections for evaluating the performance of the detection and recognition models.
- Evaluation results will be saved in the `results` folder.

### Results

- **Detection Results**: Images with drawn bounding boxes will be saved in `results/results_detection`.
- **Recognition Results**: Recognized characters and their accuracy will be saved in `results/results_recognition`.

## Contributions

Feel free to fork this repository, make your own changes, and submit pull requests. Contributions are welcome!

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
