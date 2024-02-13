# DeepFake Detection 

## Introduction
Welcome to our DeepFake Detection project! This repository focuses on detecting DeepFake videos and images using two distinct methods: Convolutional Neural Networks (CNN) and Discrete Fourier Transform (DFT) combined with Support Vector Machines (SVM).

## Table of Contents
1. [Motivation](#motivation)
2. [Installation](#installation)
3. [Usage](#usage)
4. [Dataset](#dataset)
5. [CNN Method](#cnn-method)
6. [DFT+SVM Method](#dftsvm-method)
7. [Contributing](#contributing)
8. [License](#license)

## Motivation
With the rise of deepfake technology, the need for robust detection mechanisms becomes crucial. This project aims to provide an open-source solution for identifying deepfake videos using both traditional and modern approaches. By employing CNN and DFT+SVM methods, we offer a comprehensive tool for detecting manipulated content.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/duongve13112002/DeepFakeDetection.git
   cd DeepFakeDetection
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

### CNN Method:

1. Navigate to the `CNN` directory:
   ```bash
   cd CNN
   ```

2. Run the CNN detection script:
   ```bash
   jupyter notebook app/app.ipynb
   ```

### DFT+SVM Method:

1. Navigate to the `DFT_SVM` directory:
   ```bash
   cd DFT_SVM
   ```

2. Run the DFT+SVM detection script:
   ```bash
   jupyter notebook app.ipynb
   ```

## Dataset

The deepfake detection models in this project were trained on a diverse dataset consisting of 140,000 real and fake faces, as well as the FaceForensics++ dataset.

1. [**140k Real and Fake Faces Dataset:**](https://www.kaggle.com/datasets/gauravduttakiit/140k-real-and-fake-faces)

   - This dataset comprises a collection of 140,000 images, with a balanced distribution between real and fake faces. The real faces are sourced from various public datasets, ensuring a diverse representation of genuine facial expressions and backgrounds.

2. [**FaceForensics++:**](https://github.com/ondyari/FaceForensics)

   - FaceForensics++ is an extension of the original FaceForensics dataset, specifically designed for deepfake detection research. It includes a diverse set of manipulated videos, covering various manipulation methods such as Deepfakes, Face2Face, FaceSwap, and NeuralTextures. The dataset provides a challenging environment for training and evaluating deepfake detection models due to its realistic simulations of facial manipulations.

The combination of the 140k Real and Fake Faces Dataset with FaceForensics++ ensures a comprehensive training set with a wide range of facial variations and manipulation techniques, enhancing the robustness and generalization of the deepfake detection models.


## CNN Method
The CNN (Convolutional Neural Network) method employed in this deepfake detection project utilizes the InceptionResNetV2 architecture. InceptionResNetV2 is known for its efficiency and effectiveness in image classification tasks. This method involves training the neural network on a dataset containing both authentic and deepfake videos, enabling it to learn features and patterns characteristic of deepfake content.

## DFT+SVM Method

The DFT+SVM (Discrete Fourier Transform + Support Vector Machine) method combines frequency domain analysis with machine learning to detect deepfake videos. The Discrete Fourier Transform is applied to video frames, and the resulting frequency domain representation is used to train a Support Vector Machine classifier. This method is effective in capturing subtle artifacts introduced by deepfake generation processes in the frequency domain.

## Contributing
We welcome contributions from the community to enhance our project. Whether you want to improve the model, add new features, or fix bugs, please feel free to submit pull requests.

## License
This project is licensed under the [MIT License](LICENSE) - see the [LICENSE](LICENSE) file for details.
