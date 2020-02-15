# Custom Image Classification(Fruits Classification) in Android device trained in teachablemachine with google.

<img width="1041" alt="Screen Shot 2020-02-15 at 6 57 55 PM" src="https://user-images.githubusercontent.com/10113553/74588746-30be2080-5025-11ea-82c5-f48d445240ef.png">


## Overview


Custom Image Classification to continuously classify whatever it sees from the android device's back camera.
Inference is performed using the TensorFlow Lite Java API. The demo app
classifies frames in real-time, displaying the top most probable
classifications. It allows the user to choose between a floating point or quantized model optimization.

These instructions walk you through training,building and
running the demo on an Android device. 

### Model
The training platform used for training custom image classifier is the [teachablemachine](https://teachablemachine.withgoogle.com/)
with google. This is an exciting platform for learning the deeplearning training process just at a click by just uploading the different class of dataset or using webcam, then train it quite easily.
Finally, after training you can export the model of your choice. I have exported it to tensorflowlite version as I have to run this on android device. you can choose whatever format you want and download the model.

![Training](https://user-images.githubusercontent.com/10113553/74587740-64e11380-501c-11ea-9f39-68f2dfee19a2.gif)

## Requirements
*   Image dataset of different classes(for custom training)
    (you can download the fruit dataset collected:)
    [Fruit](https://drive.google.com/file/d/12fQWCDOsEY9IXvKEg3BtbMMTnd-rOjBE/view?usp=sharing)

*   Android Studio 3.2 (installed on a Linux, Mac or Windows machine)

*   Android device in
    [developer mode](https://developer.android.com/studio/debug/dev-options)
    with USB debugging enabled

*   USB cable (to connect Android device to your computer)

## Build and run

### Step 1. Upload the dataset(custom dataset) 

Prepare and upload the dataset to the teachablemachine with google site and define the number of classes
accordingly. Train the image classification model over there and finally, export the model in the form of 
tensorflowlite format.


### Step 2. Clone this repository for image classification using deep learning

Clone this GitHub repository to your computer and save it to the folder of your choice.
This the java code for android  application.


### Step 3. Build the Android Studio project

Select `Build -> Make Project` and check that the project builds successfully.
You will need Android SDK configured in the settings. You'll need at least SDK
version 23. The `build.gradle` file will prompt you to download any missing
libraries.
you have to put the fruits.tflite to the asset folder of the android structure 
project directory and change the labels according to the number of class you have trained.


### Step 4. Install and run the app

Connect the Android device to the computer and be sure to approve any ADB
permission prompts that appear on your phone. Select `Run -> Run app.` Select
the deployment target in the connected devices to the device on which the app
will be installed. This will install the app on the device.



