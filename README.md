# Virtual-Detection-of-Freeway-Crashes-using-CV-Trajectories-and-CNN

## Description:
  This repository contains the implementation and research code for the project "Virtual Detection of Freeway Crashes Using Connected Vehicle Trajectories and Convolutional Neural Networks". The study aims to improve the detection of freeway crashes by leveraging real-time connected vehicle data and image-based trajectory classification using Convolutional Neural Networks (CNN). The approach provides a scalable, cost-effective alternative to traditional sensor-based systems by utilizing commercial connected vehicle data with a CNN model achieving a classification accuracy of over 99%.

## Key Features:
  **Data Processing**: Utilizes connected vehicle data provided by a third-party vendor, focusing on vehicle trajectories and acceleration noise near crash sites.
  
  **Image Generation**: Converts vehicle trajectory data into images for classification.
  
  **CNN Model**: A custom Convolutional Neural Network (CNN) designed to classify images into crash and non-crash situations.
  
  **Model Training**: Includes the training of the CNN model with annotated datasets of crash and non-crash trajectory images.
  
  **Evaluation**: Model evaluation with real-time crash detection on new crash events, including analysis of false positives and model performance.
  
  **Future Improvements**: Discusses potential enhancements, including better filtering to reduce false positives and the development of a high-level data pipeline for real-time applications.
  
## Methodology
  ## Data Collection:
  - Extracted crash data from Iowa DOT's Traffic Management Center (TMC) and vehicle trajectory data from Wejo.
  - Data was geo-fenced within a 2-mile radius and 2-hour window around each crash for analysis.
  ## Image Generation:
  - Generated trajectory images representing crash and non-crash situations for each freeway segment.
  - Created over 1000 labeled images for training, with 450 crash and 400 non-crash images.
  ## Model Training:
  - Developed a CNN model with three convolutional layers, followed by max pooling, flattening, and dense layers for image classification.
  - Used Adam optimizer for improved training efficiency and accuracy.
  ## Evaluation:
  - Assessed the model with a separate set of crash images to ensure robust detection capability.
  - Observed some false positives, indicating areas for improvement in real-time deployment.

## Contents:
  - **data/**: Contains sample datasets used for training and evaluation (note: data used here is synthetic due to privacy concerns).
-**crash detection.ipynb/**: Jupyter notebooks for data preprocessing, image generation, and CNN training.
-**results/**: results for model evaluation on real-time crash data.
-**docs/**: Documentation of the methodology, model architecture, and findings from the study.
-**README.md**: Overview of the project, setup instructions, and usage guidelines.
    
Requirements:
Python 3.x
TensorFlow/PyTorch for CNN implementation
Libraries: NumPy, Pandas, Matplotlib, Seaborn, OpenCV

License:
This project is licensed under the MIT License.

Acknowledgments:
We thank the Institute for Transportation and Dr. Anuj Sharma for providing the datasets used in this academic project. Special thanks to the Iowa Department of Transportation for their support.

This repository is designed to help researchers and practitioners in the field of traffic management and AI-driven safety solutions. Feel free to contribute to the project or reach out for collaboration!
