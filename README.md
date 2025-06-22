# 👤 Real-Time Face Recognition Using OpenCV & face_recognition

## 📌 Overview
This project demonstrates **real-time face recognition** using your webcam. By leveraging the `face_recognition` and `OpenCV` libraries, it identifies known faces (like Narendra Modi and Harsh Tyagi) and labels them live on the video feed.

---

## 🎯 Features
- Recognizes multiple known faces in real-time
- Draws bounding boxes and labels for each face
- Scales input for faster performance
- Easy extension to add more known faces

---

## 🧰 Libraries Used
```python
import face_recognition
import cv2
```

---

## 🛠️ How It Works
1. Load images of known people (e.g., `modi.jpg`, `harsh.jpg`)
2. Extract face encodings from these images
3. Start webcam and capture frames
4. Detect and encode faces from each frame
5. Compare detected faces to known encodings
6. Draw bounding boxes and labels around recognized faces

---

## ▶️ How to Run
1. Make sure your environment has a webcam.
2. Install dependencies:
```bash
pip install face_recognition opencv-python
```
3. Save known face images (e.g., `modi.jpg`, `harsh.jpg`) in the same directory.
4. Run the script:
```bash
python face_recognition_realtime.py
```
5. Press `q` to quit the webcam window.

---

## 📁 Folder Structure
```
├── face_recognition_realtime.py
├── modi.jpg
├── harsh.jpg
└── README.md
```

---

## 🧪 Customization
- To add more faces, load more images and append their encodings and names to the respective lists:
```python
new_image = face_recognition.load_image_file("./new_person.jpg")
new_encoding = face_recognition.face_encodings(new_image)[0]
known_face_encodings.append(new_encoding)
known_face_names.append("New Person")
```

---

## 👤 Author
**Harsh Kumar Tyagi**  
📧 [harshtyagi022@gmail.com](mailto:harshtyagi022@gmail.com)  
🪪 License: MIT
