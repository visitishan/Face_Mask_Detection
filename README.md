# 😷 Face Mask Detection 
[![Build Status](https://img.shields.io/pypi/pyversions/Django.svg?maxAge=2592000)]()

An ML based solution to detect and ensure if the people are wearing a face mask in public places using TensorFlow and Keras.

The face detection model is trained on a dataset of 686 images with human faces. And the face mask detection model is trained on a dataset of 690 images of people wearing a mask.

## How to install -

1. Install Python 3.5 or newer.
2. Clone this repository into your local machine using command - 
```
git clone https://github.com/visitishan/Face_Mask_Detection.git
```
3. Navigate to your newly created folder and create a python virtual environment using
```
python -m venv --system-site-packages .\venv
```
4. Activate the virtual environment -
```
.\venv\Scripts\activate
```
5. Install the required packages -
```
pip install -r requirements.txt
```
6. Verify the installation of TensorFlow. If a tensor is returned, it means TensorFlow is installed successfully. (Optional)
```
python -c "import tensorflow as tf;print(tf.reduce_sum(tf.random.normal([1000, 1000])))"
```

Great!! You are ready to use the code now.


## How to use -
If you want to re-train the model from the images dataset or with your custom images, you can do it by running -
```
python train_mask_detector.py --dataset dataset
```
This will save a new model file with the name mask_detector.model in the working directory.

To test the model on images, you can use the file detect_mask_image.py. Run the following command - 
```
python detect_mask_image.py --image examples/example_01.png
```
Here we are running the code for a test image stored in the examples folder. You can change the argument value with the path of your custom image to test.

To detect face mask on a continuous video stream from your webcam, you can run -
```
python detect_mask_video.py
```


## Screenshots -
Yet to be captured and updated 😉

