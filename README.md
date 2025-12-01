# MSBA 503 Take-Home Assignment – Computer Vision Object Detection

## Overview
This project applies two deep learning object detection models—**Faster R-CNN** and **RetinaNet**—to a set of 10 images in order to compare their performance. The comparison focuses on three key metrics required in the assignment:  
1. Number of objects detected  
2. Average and maximum confidence scores  
3. Inference (processing) time per image  

Additionally, a **ResNet-50 image classification model** is used to extract the top predicted label and probability for each image as part of Part A(ii).

All work for Parts A(i) and A(ii) is included in the Jupyter notebook.

---

## Models Used
### **1. Faster R-CNN (ResNet-50 FPN)**
- Pretrained on the COCO dataset  
- High accuracy  
- Slower inference time  
- Often detects more objects at higher confidence  

### **2. RetinaNet (ResNet-50 FPN)**
- Also pretrained on COCO  
- Faster inference  
- Sometimes detects fewer objects  
- Good real-time trade-off model  

### **3. ResNet-50 Classification Model**
- Used for extracting the top predicted image class and probability  
- Complements the object detection outputs with a single high-level label  

---

## Project Structure


> **Note:** Images are **not uploaded** to GitHub per assignment instructions. They are expected to be placed in the same directory as the notebook when running the project.

---

## How to Run

1. Install required libraries (run these in terminal, not inside the notebook):
   ```bash
   pip install torch torchvision torchaudio
   pip install pandas pillow matplotlib
