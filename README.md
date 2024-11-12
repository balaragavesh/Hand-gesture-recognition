# Hand Gesture Recognition

This project enables real-time hand gesture recognition using **MediaPipe** and **OpenCV**. The system can detect and classify gestures from both hands simultaneously, making it ideal for applications requiring multi-hand gesture recognition. This README provides a step-by-step guide on how to set up, collect data, and start recognizing gestures.

## Features

- **Real-time hand gesture recognition** for both right and left hands.
- Utilizes **MediaPipe** for hand landmark detection and **OpenCV** for video capture.
- **Customizable gesture classes**, allowing you to create a unique dataset of gestures for specific applications.
- Outputs data in a structured format for **easy training and model development**.

## Getting Started

Follow the steps below to set up and run the project.

### Prerequisites

Ensure you have **Python 3.x** installed. This project also requires several libraries, which can be installed via the `requirements.txt` file.

### Installation

1. **Clone the Repository**

   ```bash
   git clone https://github.com/yourusername/hand-gesture-recognition.git
   cd hand-gesture-recognition
   ```

2. **Install Required Libraries**

   Install the required libraries using the following command:

   ```bash
   pip install -r requirements.txt
   ```

   This will install dependencies like `mediapipe` and `opencv-python`.

## Data Collection

To create your own dataset of hand gestures, use the provided Jupyter notebook `Data_collection.ipynb`.

1. **Open the Notebook**

   Open `Data_collection.ipynb` in Jupyter Notebook or JupyterLab.

2. **Configure Class Labels**

   In the notebook, specify the class label for each gesture by modifying the `class_name` variable. This allows you to collect data for different gestures separately.

3. **Collect Data for Each Gesture**

   - Run the notebook cell to start collecting data.  
   - Ensure that gestures for both the **right hand** and **left hand** are captured in separate datasets. The notebook will automatically combine data from both hands into a single CSV file for easy access and use in training.

   **Note**: Make sure to capture sufficient data for each gesture to ensure accurate model performance.

4. **Output**

   The collected data will be saved in a `.csv` format, with landmarks for each hand gesture. This dataset can be used to train a machine learning model for gesture recognition.

## Running the Gesture Recognition System

After collecting data, you can run the gesture recognition model to detect gestures in real-time. A sample code for loading your data and testing gestures on live video feed will be provided in a separate script.

## Customization

- **Add more gestures**: You can add more gestures by creating new class labels and collecting additional data.
- **Model fine-tuning**: The model can be fine-tuned or modified based on specific applications, such as sign language recognition, gaming, or hands-free control interfaces.

## Future Improvements

- **Deep learning integration**: Integration with deep learning models for more accurate gesture classification.
- **Complex gestures and sequences**: Support for recognizing more complex gestures and gesture sequences.
- **Edge optimization**: Optimization for faster real-time processing on edge devices.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
