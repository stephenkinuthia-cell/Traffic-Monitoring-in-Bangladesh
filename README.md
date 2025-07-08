# 🚦 Traffic Monitoring in Bangladesh

## 📘 Project Overview

This project is focused on real-time object detection in traffic video feeds from Dhaka, Bangladesh. Using the YOLO (You Only Look Once) object detection model, I detect and classify vehicles and pedestrians from both images and video data. The project walks through each key stage—from video frame extraction to custom model training—providing a hands-on understanding of how to build, train, and deploy object detection systems.

---

## 📚 Table of Contents

- [Lesson 1: Working with File System Paths](#lesson-1-working-with-file-system-paths)
- [Lesson 2: Working with Image and Video Data](#lesson-2-working-with-image-and-video-data)
- [Lesson 3: Object Detection with YOLO](#lesson-3-object-detection-with-yolo)
- [Lesson 4: Training YOLO for Custom Classes](#lesson-4-training-yolo-for-custom-classes)
- [Lesson 5: Data Augmentation for Object Detection](#lesson-5-data-augmentation-for-object-detection)
- [Lesson 6: The Self-Driving Trolley Problem](#lesson-6-the-self-driving-trolley-problem)
- [License](#license)
- [Contact](#contact)

---

## 📘 Lesson 1: Working with File System Paths

### 🮾 Summary

In this lesson, I learned how to work with file system paths using Python's `pathlib` module. This module provides a modern, object-oriented approach for handling file paths and directory operations.

### 🎯 Objectives

- Use `pathlib` to manage file paths
- Create and organize folders
- Traverse directories
- Filter files based on patterns

### 🧪a Example Code

```python
from pathlib import Path

path = Path("data/videos")
if path.exists():
    print("Path exists!")

for video_file in path.glob("*.mp4"):
    print(video_file.name)

Path("data/frames").mkdir(parents=True, exist_ok=True)
```

---

## 📸 Lesson 2: Working with Image and Video Data

### 🮾 Summary

I explored how to work with image and video data for object detection using a traffic dataset. This involved extracting frames, parsing bounding box annotations, and visualizing object locations.

### 🎯 Objectives

- Load and organize the dataset
- Extract frames from videos
- Parse XML annotations
- Visualize bounding boxes on images

### 📚 New Terms

- Bounding Boxes
- Frame Rate
- XML

### ✅ Conclusion

I can now prepare datasets by extracting and labeling frames from videos, which sets the foundation for object detection.

---

## 🧠 Lesson 3: Object Detection with YOLO

### 🮾 Summary

I used the pre-trained YOLO model to perform object detection on both images and videos. This included parsing YOLO outputs and drawing bounding boxes.

### 🎯 Objectives

- Use YOLO to detect objects in images and videos
- Visualize detection results
- Handle directories and video inputs

### 📚 New Terms

- Object Detection
- YOLO
- Bounding Boxes
- Normalized Coordinates

### ✅ Conclusion

I learned how to apply YOLO to real data sources and interpret its output for further use.

---

## 🧪 Lesson 4: Training YOLO for Custom Classes

### 🮾 Summary

I fine-tuned a pre-trained YOLO model to detect custom object classes. This involved converting annotations, organizing data, and running training loops.

### 🎯 Objectives

- Convert XML to YOLO format
- Structure dataset folders
- Handle malformed data
- Train YOLO to detect new classes

### 📚 New Term

- YAML

### ✅ Conclusion

I can now train YOLO to detect any object class I care about, using transfer learning and properly structured datasets.

---

## 🧬 Lesson 5: Data Augmentation for Object Detection

### 🮾 Summary

I implemented data augmentation techniques to improve model generalization. I used Torchvision to transform images and adjusted bounding boxes accordingly.

### 🎯 Objectives

- Explore YOLO’s internal augmentation
- Use Torchvision transforms
- Adjust bounding boxes
- Chain multiple augmentation techniques

### 📚 New Term

- Data Augmentation

### ✅ Conclusion

Data augmentation has made my dataset more diverse and helped improve training robustness for custom object detection.

---

## 🚗 Lesson 6: The Self-Driving Trolley Problem

### 🮾 Summary

I explored the ethical dimensions of AI through the self-driving trolley problem. I reflected on how values encoded in AI can impact real-world outcomes.

### 🧐 Key Ideas

- AI lacks moral consciousness
- Decisions reflect developer biases
- Global ethical standards are needed

### ✅ Conclusion

As I build AI systems, I must remain aware of the ethical impact and strive to design models that are fair, transparent, and responsible.

---

## 📄 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## 📬 Contact

**Stephen Kinuthia**\
📧 Email: [kinuthiastephen94@gmail.com](mailto\:kinuthiastephen94@gmail.com)\
🌐 GitHub: [github.com/stephenkinuthia-cell](https://github.com/stephenkinuthia-cell)

Feel free to reach out for feedback, questions, or collaboration opportunities!

