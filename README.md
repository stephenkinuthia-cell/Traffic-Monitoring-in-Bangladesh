## 🛣️ AI Lab 03: Traffic Monitoring in Bangladesh

### 📌 Overview

In this project, you'll be working with **traffic video feed data from Dhaka, Bangladesh**. The main goal is to **analyze real-time traffic footage** by detecting and labeling objects such as **cars, people, motorcycles**, and more in each video frame.

You will use a combination of a **pre-trained YOLO (You Only Look Once) object detection model** and train a **custom YOLO model** to recognize new objects that are specific to the dataset or region. This enables more accurate and localized traffic analysis.

---

### 🎯 Learning Outcomes

By the end of this project, you will be able to:

- ✅ **Work with XML data** containing object bounding boxes (typically in Pascal VOC format).
- ✅ **Extract individual frames** from video files using Python tools like `OpenCV`.
- ✅ **Apply a pre-trained YOLO model** to detect common objects in images and video frames.
- ✅ **Train YOLO for custom object detection**, including annotation and dataset preparation.
- ✅ **Use data augmentation techniques** to increase the diversity and quality of your training dataset, improving your model’s generalization ability.

---

### 🧠 Skills & Technologies Involved

- Python Programming
- Computer Vision
- Deep Learning (YOLO Object Detection)
- OpenCV
- Data Preprocessing & Augmentation
- Annotation Formats (XML → YOLO)
- Real-time Video Processing

---

> ⚙️ This lab is a strong foundation for real-world applications such as traffic management systems, vehicle tracking, and intelligent surveillance in urban areas.

## 📘 Lesson 1: Working with File System Paths using `pathlib`

### 🧾 Overview

In this lesson, you'll learn how to work with file system paths in Python using the modern and powerful `pathlib` module. This module provides a more elegant, readable, and object-oriented way to manage file paths compared to the traditional `os.path` approach.

---

### 🧠 Key Concepts

- `pathlib` treats file paths as **objects**, not strings.
- It provides **cross-platform compatibility** for file operations (Windows, Linux, macOS).
- Offers methods to perform common file tasks such as:
  - Listing directory contents
  - Creating directories
  - Searching for files
  - Checking path existence

---

### 🛠️ Why Use `pathlib`?

- ✅ Cleaner syntax
- ✅ Better code readability
- ✅ Integrated object-oriented methods
- ✅ Consistent behavior across platforms

---

### 🧪 Example Usage

```python
from pathlib import Path

# Create a Path object
path = Path("data/videos")

# Check if the path exists
if path.exists():
    print("Path exists!")

# List all .mp4 files in the directory
for video_file in path.glob("*.mp4"):
    print(video_file.name)

# Create a new directory (if it doesn't exist)
Path("data/frames").mkdir(parents=True, exist_ok=True)
