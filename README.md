# Object Detection for Face Recognition using Detectron2 in Python

## Table of Contents
- [Overview](#overview)
- [Tech Stack](#tech-stack)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Setup](#setup)
- [Usage](#usage)
- [Model Training and Evaluation](#model-training-and-evaluation)
- [Results and Visualizations](#results-and-visualizations)
- [Contributing](#contributing)
- [License](#license)

## Overview
This project focuses on object detection for face recognition using Detectron2, a powerful library built on PyTorch. The model is trained to detect faces in images, and the dataset is obtained from a face detection dataset provided by Johns Hopkins University Center for Systems Science and Engineering (JHU CSSE). The goal is to develop a robust face detection system.

## Tech Stack
- Detectron2
- PyTorch
- OpenCV
- Pandas

## Dataset
The face detection dataset is sourced from JHU CSSE, containing images with annotated face regions. The images are processed and annotated, and the dataset is split into training and testing sets for model evaluation.

## Project Structure
/faces
Contains original images
/annotated_results
Contains images with annotated faces
annotations.csv
CSV file containing image annotations
detectron2_face_detection.ipynb
Jupyter Notebook with the project code
face_detector.pth
Pre-trained face detection model weights
requirements.txt
List of project dependencies

## Setup
To set up the project, follow these steps:
1. Install the required dependencies using `pip install -r requirements.txt`.
2. Download the face detection dataset and place the images in the `/faces` directory.
3. Run the Jupyter Notebook (`detectron2_face_detection.ipynb`) to train and evaluate the model.

## Usage
- The trained model can be used for face detection in new images.
- Check the Jupyter Notebook for detailed usage examples and code snippets.

## Model Training and Evaluation
The object detection model is trained using the Detectron2 framework with the mask_rcnn_X_101_32x8d_FPN_3x architecture. The training process involves configuring the model, setting hyperparameters, and training on the prepared dataset. The model is evaluated on a validation set using the COCOEvaluator to assess its performance.

## Results and Visualizations
The trained model is used to make predictions on the test set, and the results are visualized. Annotated images are generated with bounding boxes around detected faces, showcasing the model's accuracy. Sample annotated images are provided for reference.

## Contributing
Contributions are welcome! If you have any suggestions, bug reports, or improvements, feel free to open an issue or create a pull request.

## License
This project is licensed under the [MIT License](LICENSE).
