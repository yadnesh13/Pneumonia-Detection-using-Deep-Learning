# Pneumonia Detection Using Deep Learning

## Overview

This project aims to create a web application for detecting pneumonia from chest X-ray images using a convolutional neural network (CNN) model built with TensorFlow and Keras. The web interface allows users to upload chest X-ray images and receive predictions on whether the patient has pneumonia, along with the model's confidence in the prediction.

## Features

- **Image Upload**: Users can upload chest X-ray images via the web interface.
- **Real-time Predictions**: The application processes the uploaded image and provides a prediction indicating whether the patient has pneumonia.
- **Confidence Score**: Alongside the prediction, the model's confidence is displayed, giving users insight into the certainty of the diagnosis.
- **User-friendly Interface**: Simple and intuitive web interface built with Flask for easy interaction.

## Project Structure

```
project/
│
├── app.py                   # Main Flask application
├── templates/
│   ├── index.html           # HTML template for image upload
│   └── result.html          # HTML template for displaying prediction results
└── uploads/                 # Directory to store uploaded images
```

## Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/your-username/pneumonia-detection.git
    cd pneumonia-detection
    ```

2. **Create a virtual environment and activate it**:
    ```bash
    python -m venv venv
    source venv/bin/activate   # On Windows, use `venv\Scripts\activate`
    ```

3. **Install the required packages**:
    ```bash
    pip install -r requirements.txt
    ```

4. **Download the pre-trained model**:
    - Place the pre-trained model file (`your_model.h5`) in the project directory.

## Usage

1. **Run the Flask application**:
    ```bash
    python app.py
    ```

2. **Open your web browser and navigate to** `http://127.0.0.1:5000/`.

3. **Upload a chest X-ray image** using the provided form.

4. **View the prediction results** indicating whether the patient has pneumonia and the model's confidence score.

## Model Training

The CNN model was trained on the [Chest X-ray dataset](https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia) from Kaggle. The dataset contains labeled images of chest X-rays categorized into 'PNEUMONIA' and 'NORMAL' classes. The model architecture includes several convolutional layers followed by max-pooling layers, and a final dense layer with a sigmoid activation function to output the probability of pneumonia.

## Dependencies

- TensorFlow
- Keras
- Flask
- OpenCV
- NumPy
- Matplotlib

## Contributing

Contributions are welcome! If you have any suggestions or improvements, feel free to create a pull request or open an issue.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Acknowledgements

- Special thanks to the authors of the Chest X-ray dataset available on Kaggle.
- Inspiration and guidance from various online resources and deep learning communities.

---

Feel free to adjust the description to better fit your project's specifics, such as adding any additional dependencies or acknowledgments.
