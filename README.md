# Signature Verification and Personality Prediction

This repository contains all the necessary components for a signature verification and personality prediction system. The project consists of two main parts: 
1. A classification model for verifying the authenticity of signatures.
2. Prediction of the personality based on the signature.
3. A connection setup between a Colab notebook and a mobile app for real-time predictions.

- **archive**: Contains the dataset used for training and testing the models.
- **models**: Contains the trained models and a JSON file with class indices.
- **notebooks**: 
  - [signature personaltiy prediction3.ipynb](https://github.com/daivik05/signature_personality_prediction/blob/main/signature_personality_prediction.ipynb): Notebook for creating and training the classification model.
  - [sign_test_2.ipynb](https://github.com/daivik05/signature_personality_prediction/blob/main/sign_test_2.ipynb): Notebook for setting up the connection between Colab and the mobile app. This file also has the personality prediction code.
- **README.md**: This file.


## Getting Started

### Prerequisites

- Google Colab
- Python 3.x
- TensorFlow
- Keras
- OpenCV
- Flask
- ngrok

### Usage

#### 1. Setting Up the Classification Model

Open the `signature personaltiy prediction3.ipynb` notebook in Google Colab and run the cells to create and train the signature verification model. The notebook includes the following steps:

1. Load and preprocess the dataset.
2. Define and compile the model.
3. Train and evaluate the model.
4. Save the trained model as `signature personaltiy prediction3.ipynb`.

#### 2. Connecting to the Mobile App

Open the `sign_test_2.ipynb` notebook in Google Colab and follow the instructions to set up the connection between Colab and the mobile app. The notebook includes:

1. Loading the pre-trained model (`signature personality prediction3.h5`).
2. Setting up a Flask server to handle image uploads and return predictions.
3. Using ngrok to create a public URL for the Flask server.
4. Instructions to connect the mobile app to this URL for real-time predictions.

### Dataset

The dataset used for training and testing is located in the `archive` directory. It contains separate folders for training, testing, and validation. The dataset that has been used for this project was downloaded from [`Kaggle`](https://www.kaggle.com/datasets/robinreni/signature-verification-dataset).

### Models

The pre-trained models are located in the `models` directory:

- `signature personality prediction3.h5`: Model for signature verification.
- `sign_test_2.ipynb`: Code for personality prediction as well as flask connection.
- `class_indices.json`: JSON file mapping class labels to indices.

### Mobile App

The mobile app is designed to upload images to the Flask server and display the prediction results. Ensure you have set up the app to point to the ngrok URL generated in the `sign_test_2.ipynb` notebook.
The basic code for the mobile app is available in this repository: [signature_verification_app](https://github.com/daivik05/signature_verification_app). This app is designed to upload images to the Flask server and display the prediction results. Ensure you have set up the app to point to the ngrok URL generated in the `sign_test_2.ipynb` notebook.


## Contributing

Feel free to open issues or submit pull requests for any improvements or bug fixes.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.



