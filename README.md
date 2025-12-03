1. Project Title

Object Detection on Real-World Images Using RetinaNet and Faster R-CNN

2. Project Overview

This project applies modern computer vision models to detect objects in real-world images. I use two deep learning object-detection algorithms — RetinaNet and Faster R-CNN — to analyze 10 images collected online and compare their ability to identify objects, confidence levels, and inference speed. The results highlight how different architectures behave on the same inputs and which model performs best in everyday detection scenarios.

3. Objectives

Use two deep learning algorithms for object detection

Run predictions on 10 real-world images

Compare the models across:

Number of objects detected

Confidence probabilities

Inference runtime

Consistency of detections

Summarize the results in a comparison table

Provide short, clear insights (as required by professor)

4. Models Used
Model 1 — RetinaNet

Pretrained on the COCO dataset

Known for high accuracy with focal loss

Good at detecting small objects

Model 2 — Faster R-CNN

Pretrained on COCO

Two-stage detector with region proposals

Typically more accurate but slower

5. Dataset (Images Used)

10 real images gathered online

Contain objects such as: people, animals, vehicles, household items, etc.

No manual labeling was done — models rely on COCO pretrained classes

All images stored in the /images/ folder

6. Methods
6.1 Preprocessing

Loaded images with OpenCV/Pillow

Resized based on model requirements

Converted images into tensors for inference

6.2 Prediction Process

For each image:

Run RetinaNet

Run Faster R-CNN

Extract:

Predicted object names

Bounding box coordinates

Confidence scores

Runtime per model

6.3 Evaluation Metrics

Models are compared using:

Object count (how many objects detected)

Average confidence

Inference speed

Qualitative accuracy (how correct were the detections?)

7. Code Structure
/project
    ├── images/
    │     ├── img1.jpg
    │     ├── img2.jpg
    │     └── …
    ├── detection_loop.py
    ├── retina.py
    ├── faster_rcnn.py
    ├── results.csv
    └── Final_Project.ipynb


8. Insights & Limitations

Pretrained models may misidentify rare objects not in COCO

Faster R-CNN is slower but more accurate

RetinaNet is better for lightweight applications

Image lighting and angles affect detection quality

9. Conclusion

This project demonstrates how modern computer vision models detect objects in everyday images.
Faster R-CNN typically offers higher accuracy, while RetinaNet provides faster performance.
Using both models allowed for a robust comparison of speed, precision, and confidence.

