## TrainYourOwnYOLO

This repo let's you train a custom image detector using the state-of-the-art YOLOv3 computer vision algorithm.This repo works with TensorFlow 2.3 and Keras 2.4.

## To build and test your YOLO object detection algorithm follow the below steps:

### Image Annotation
1. Install Microsoft's Visual Object Tagging Tool (VoTT)
2. Annotate images
### Training
1. Download pre-trained weights
2. Train your custom YOLO model on annotated images
### Inference
1. Detect objects in new images and videos

## GitHub Repository structure
### 1_Image_Annotation: 
Scripts and instructions on annotating images
### 2_Training: 
Scripts and instructions on training your YOLOv3 model
### 3_Inference: 
Scripts and instructions on testing your trained YOLO model on new images and videos
### Data: 
Input Data, Output Data, Model Weights and Results
### Utils: 
Utility scripts used by main scripts

## Testing Your Detector
To detect objects run the detector script from within the [`TrainYourOwnYOLO/3_Inference`](/3_Inference/) directory:.
```
python Detector.py
```
The outputs are saved to [`TrainYourOwnYOLO/Data/Source_Images/Test_Image_Detection_Results`](/Data/Source_Images/Test_Image_Detection_Results). The outputs include the original images with bounding boxes and confidence scores as well as a file called [`Detection_Results.csv`](/Data/Source_Images/Test_Image_Detection_Results/Detection_Results.csv) containing the image file paths and the bounding box coordinates. For videos, the output files are videos with bounding boxes and confidence scores. For real-time detection use `python Detector.py --webcam` this will open up your webcam and detect your data classes. To list available command line options run `python Detector.py -h`.

#### Thank you
