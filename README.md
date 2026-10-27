
# Facial Emotion Recognition Using CNN

A deep learning project that recognizes facial expressions from images using a Convolutional Neural Network (CNN) built with TensorFlow and Keras.

## Features

- Facial image preprocessing and normalization
- CNN-based emotion classification
- Training and validation accuracy monitoring
- Early stopping to help prevent overfitting
- Saving the trained model for future predictions
- Saving emotion class names in JSON format

## Technologies Used

- Python
- TensorFlow and Keras
- NumPy
- Matplotlib
- Google Colab

## Project Structure

```text
Facial-Emotion-Recognition/
├── facial_emotion_recognizer.ipynb
├── README.md
├── best_fer_model.keras
└── class_names.json
```

**Note:** The trained model and class names are generated after training. They are not automatically included in the repository.

## Model Architecture

The CNN model uses:

1. Convolutional layers for feature extraction
2. Batch normalization
3. Max pooling
4. Global average pooling
5. Dense layers for classification
6. Dropout for regularization
7. Softmax for emotion classification

## Dataset

The model expects facial images organized into training and validation folders, with a separate subfolder for each emotion class.

```text
fer_data/
└── images/
    ├── train/
    │   ├── emotion_1/
    │   └── emotion_2/
    └── validation/
        ├── emotion_1/
        └── emotion_2/
```

The notebook loads the class names from the training directory structure.

The dataset is not included in this repository.

## Installation

Install the required packages:

```bash
pip install tensorflow numpy matplotlib pillow
```

## How to Run

1. Open `facial_emotion_recognizer.ipynb` in Google Colab.
2. Upload your dataset to Google Drive.
3. Update the dataset path if required.
4. Run the notebook cells in order.
5. Train and evaluate the model.
6. Save the trained model and class names.
7. Run app.py locally in terminal
8. A web interface using Streamlit will open .

## Output Files

| File | Description |
|---|---|
| `best_fer_model.keras` | Saved trained CNN model |
| `class_names.json` | Emotion class labels |

## Future Improvements

- Real-time emotion recognition using a webcam
- Evaluation using a confusion matrix, precision, and recall
- Deployment as a web application

## Limitations

Predictions may be affected by lighting, image quality, facial pose, and dataset diversity. Facial expressions do not necessarily indicate a person's actual emotional state.


Add a suitable license if you intend to distribute this project.
