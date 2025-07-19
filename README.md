Image Classifier AI

Image Classifier AI is a web application built with Streamlit that allows users to upload an image and classify its contents using a pre-trained MobileNetV2 deep learning model. The app leverages TensorFlow Keras's MobileNetV2 model trained on ImageNet to provide the top-3 predictions of the image content.
Features

    Upload images in JPG or PNG format.

    Real-time image classification with MobileNetV2.

    Display of uploaded image for confirmation.

    Top-3 predicted labels with confidence scores.

    Error handling for image processing or prediction issues.

Technologies Used

    Python 3

    Streamlit for web interface

    TensorFlow Keras for deep learning model (MobileNetV2)

    OpenCV and NumPy for image preprocessing

    Pillow for image loading

Installation

    Clone the repository or download the project files.

    Install the required Python packages:

bash
pip install streamlit tensorflow opencv-python pillow numpy

Usage

Run the Streamlit app from your terminal:

bash
streamlit run your_script_name.py

This will launch a local web server and open the app in your browser.
How to Use

    Click the "Choose an image..." button to upload a JPG or PNG image.

    The uploaded image will be displayed.

    Click the "Classify Image" button to start prediction.

    The app will show the top-3 identified labels with their confidence percentages.

Code Overview

    load_model(): Loads the pre-trained MobileNetV2 model with ImageNet weights.

    preprocess_image(image): Converts the input image to the format required by the model (resized to 224x224 pixels, preprocessed pixel values).

    classify_image(model, image): Processes the image and generates predictions with confidence scores.

    main(): Core Streamlit app that manages UI, model loading, and user interactions.

Contributing

Contributions are welcome. Please fork the repository and submit a pull request for any feature enhancements or bug fixes.
