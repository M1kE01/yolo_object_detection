# Simplified YOLO Model Reproduction

## Overview
This project is an exploration into the realm of object detection, particularly focusing on reproducing the architecture of the renowned YOLO (You Only Look Once) model. Our approach simplifies the original YOLO model in terms of the number of layers and neurons in the Convolutional Neural Network (CNN). The primary objective was to emulate YOLO's architecture and to observe its performance in object detection tasks.

## Dataset
Unlike the original YOLO model, which utilizes the complex COCO dataset, our experiments were conducted using the Pascal VOC 2012 dataset. This dataset is smaller and more manageable, making it suitable for our simplified model.

## Model Architecture
We experimented with two different CNN architectures:
1. **Basic Model**: Comprising three convolutional layers.
2. **Enhanced Model**: Similar to the Basic Model but includes batch normalization in its convolutional layers.

Both models were designed to mirror the core aspects of the YOLO model's architecture, albeit in a more simplified form.

## Results and Observations
The models showed promising results in terms of training and object detection capabilities. Although the object detection was relatively successful, the classification accuracy was modest. A notable skew in the dataset, with 'person' objects being three times more frequent than other classes, led to a bias in predictions towards the 'person' class.

## Challenges and Future Work
The predominant challenge lies in the simplified architecture of our CNN, which doesn't capture the complexity and depth of the original YOLO model. This limitation is evident in the classification performance and the generalization capabilities of the model.

To address the data imbalance, techniques such as oversampling and undersampling could be employed. Future iterations of the project should also explore more complex and deeper CNN architectures to enhance performance.

## Additional Features
- Implementation of a custom Non-Maximum Suppression (NMS) function for improved object recognition.
- Modifications to visualize predictions from multiple models on the same image, facilitating comparative analysis.

## Usage
The project includes Python scripts for model training, preprocessing, prediction decoding, and visualization of results. The modified `draw_boxes` function allows for simultaneous visualization of results from different models on the same image.

## Contributing
Contributions to this project are welcome. Feel free to fork the repository, make changes, and submit pull requests. If you encounter any issues or have suggestions, please open an issue in the repository.

## Acknowledgments
This project is inspired by the original YOLO model and aims to provide an educational insight into the workings of object detection models.
