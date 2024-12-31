# Feature Extraction from Remote Sensing High Resolution Data using AI/ML

This problem statement was a part of Bharatiya Antariksh Hackathon organised by ISRO, to which we were the finalists of it.

### 🎯 Goal
Develop an advanced AI/ML based Feature Extraction solution from Remote Sensing High Resolution Data with three levels of outputs – tags, bounding boxes and masks.

### 🧵 Dataset
The dataset has been created by our team. It was collected from different resources like Kaggle, Google earth and ISRO Bhoonidhi.
The dataset has 5 classes : 
1) Electric Substation                    
2) High Tension Tower                     
3) Windmill
4) Farmbunds
5) Brick Kiln

Below are the images of the electric substation and brick kiln

![Screenshot 2024-12-31 162948](https://github.com/user-attachments/assets/33891015-384c-4787-81ca-10cb7a59b2ca)
![Screenshot 2024-12-31 162857](https://github.com/user-attachments/assets/c126dc91-7527-40c9-8a41-62151478edc5)                             

### 🧾 Objectives
- Dataset preparation with three levels of labels – image-level, bounding boxes and masks
- Model(s) development for Multi-label classification, localization and segmentation tasks.
- Post-processing techniques to correct any noise in the model segmentation outputs.

### 🚀 Model Implemented
We have used the Detectron 2 model because it is very good in tasks like instance segmentation and it's inference time is also very fast compared to other models. Inside of Detectron 2 we have used mask-rcnn with resnet-101 base model. People can experiment with other base models of detectron 2 which are available at : https://github.com/facebookresearch/detectron2/blob/main/MODEL_ZOO.md

### 📈 Results

![Screenshot 2024-12-31 161930](https://github.com/user-attachments/assets/484e98a1-ab37-4521-819f-c96d19152a50)
![Screenshot 2024-12-31 161745](https://github.com/user-attachments/assets/0c3d99e9-3624-4c79-a4a4-12c80c8767f8)

### 📢 Future Work
The model performance can be increased by increasing the data. The data annotation needs to be done properly was this purpose. 
Different models and techniques can be experimented for the improvement of the performance metrics. Like we were trying the approach of Yolov8 + SAM(Segment Anything Model), but we weren't able to pass proper coordinates of bounding box for proper segmentation.

### ✒️ Team : Pragati
- Abhijeet Kaithwas
- Shreyash Verma
- Rishikesh Dwivedi
