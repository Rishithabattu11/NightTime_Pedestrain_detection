## 🚶‍♂️Nighttime Pedestrian Detection Based on a Fusion of Visual Information and Millimeter-Wave Radar
---

## 📌 Overview
This project implements a **nighttime pedestrian detection system** that fuses **infrared vision information** with **millimeter-wave (MMW) radar data** to improve detection accuracy in low-visibility conditions.  
The system leverages an improved **YOLOv5 deep learning model** along with **Extended Kalman Filtering (EKF)** for robust localization and multimodal decision-level fusion.

---

## 🚀 Project Workflow & Output 

The system follows these main stages:
<br>


**1.Dataset Loading**
<br>
Pedestrian dataset (infrared images) is uploaded.
<br>
Example: 2,199 images detected in the dataset.
<br>
Dataset is then pre-processed and split into training (80%) and testing (20%).
<br>

<img width="940" height="583" alt="image" src="https://github.com/user-attachments/assets/9481a071-196a-41ee-a619-488f25f141a0" />
<br>



**2.Dataset Preprocessing**
<br>
Images are shuffled, resized, and normalized.
<br>
Splitting for training and testing is performed.
<br>
Example split: 1759 training images and 440 testing images.
<br>

<img width="940" height="583" alt="image" src="https://github.com/user-attachments/assets/d805800c-7942-47fc-8af6-5fb95efed1a4" />
<br>

**3.Model Training & Evaluation**
<br>
_Faster R-CNN_
<br>
Standard detection algorithm.
<br>
Achieved 77% accuracy on nighttime pedestrian detection.
<br>
<img width="940" height="584" alt="image" src="https://github.com/user-attachments/assets/64c00ae9-241a-4228-92f7-7f0849e6b7eb" />
<br>


_Improved YOLOv5_
<br>
Modified YOLOv5 with additional squeezing layer.
<br>
Achieved 96% accuracy.
<br>
<img width="940" height="587" alt="image" src="https://github.com/user-attachments/assets/3f855b7a-301f-4e77-9cc3-52095e443ed0" />
<br>


_Extended YOLOv6_
<br>
Latest YOLOv6 model trained on the dataset.
<br>
Achieved 99% accuracy.
<img width="940" height="589" alt="image" src="https://github.com/user-attachments/assets/4917a622-fb55-4e3b-a95a-b7ad28d6706f" />



**4.Performance Comparison**
<br>
Comparative graph showing accuracy and metrics of Faster R-CNN, YOLOv5, and YOLOv6.
<img width="940" height="584" alt="image" src="https://github.com/user-attachments/assets/3926dca3-941a-41e0-b920-83184707ffa9" />
<br>

**5.Accuracy & Loss Curves**
<br>
Training vs. Epoch curves for all models.
<br>
Green = Faster R-CNN, Blue = YOLOv5, Yellow = YOLOv6.
<img width="940" height="592" alt="image" src="https://github.com/user-attachments/assets/86ef4caa-d7eb-4517-8454-413585bec369" />
<br>


**6.Prediction on Test Data**
<br>
The trained models are used to detect pedestrians in infrared test images.
<br>
Bounding boxes are drawn around pedestrians with detection probability.
<img width="940" height="589" alt="image" src="https://github.com/user-attachments/assets/854c12bb-b2f6-4151-a093-0b97263b060e" />
<img width="940" height="583" alt="image" src="https://github.com/user-attachments/assets/8504bab3-2c8c-49b0-8a09-a1f63cc2af17" />





