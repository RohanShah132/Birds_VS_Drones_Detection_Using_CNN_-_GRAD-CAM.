
# Birds VS Drones Detection Using CNN - GRAD-CAM

This project aims to develop a Convolutional Neural Network (CNN) model to classify images of birds and drones. The model is enhanced with the GRAD-CAM technique for visual explainability, helping to interpret the decisions made by the neural network.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Model Architecture](#model-architecture)
- [Training](#training)
- [Evaluation](#evaluation)
- [Results](#results)
- [License](#license)
- [Acknowledgements](#acknowledgements)

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/RohanShah132/Birds_VS_Drones_Detection_Using_CNN_-_GRAD-CAM.git
   cd Birds_VS_Drones_Detection_Using_CNN_-_GRAD-CAM
   ```

2. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. Prepare your dataset by placing the images in the appropriate directory structure.
2. Run the training script to train the model:
   ```bash
   python train.py
   ```
3. After training, evaluate the model performance using:
   ```bash
   python evaluate.py
   ```
4. For visual explanations, use the GRAD-CAM script:
   ```bash
   python grad_cam.py
   ```

## Model Architecture

The model is based on the ResNet50V2 architecture, leveraging transfer learning to improve performance. The last few layers are modified to adapt to the binary classification problem of distinguishing between birds and drones.

## Training

The model is trained using the Adam optimizer with a learning rate of 0.0001, utilizing data augmentation techniques to enhance generalization. Class weights are computed to address class imbalance in the dataset.

## Evaluation

The model's performance is evaluated using metrics such as accuracy, precision, recall, and F1-score. A confusion matrix is plotted to visualize classification performance.

## Results

The project includes detailed plots of training and validation accuracy and loss, along with a confusion matrix and classification report, summarizing the model's effectiveness.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements

- TensorFlow and Keras for the deep learning framework.
- OpenCV for image processing tasks.
- Matplotlib and Seaborn for visualizations.
```
