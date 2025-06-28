
# 👁️‍🗨️ Real-Time Object Detection Using Haar Cascades

**Author**: A. Kabilesh Rajaselvan
**Reg. No**: 21MIA1132
**Institution**: VIT Chennai – SCOPE School
**Course**: Image and Video Analytics Lab (IVA)


---

## 🧠 Objective

To perform **real-time object detection** using OpenCV's **Haar Cascade Classifiers** for face and eye detection through webcam video stream.

---

## 🎯 Key Concepts

* Computer Vision
* Real-time Video Processing
* Haar Cascade Classifiers
* OpenCV Video Capture
* Object Detection & ROI (Region of Interest)

---

## 🛠️ Tools & Libraries Used

* Python
* OpenCV (`cv2`)
* Pre-trained Haar Cascade XML files (`haarcascade_frontalface_default.xml`, `haarcascade_eye.xml`)

---

## 📁 File Structure

```
📦 IVA_Lab_2
 ┣ 📜 IVA_LAB_2.ipynb   # Main notebook for face and eye detection
 ┗ 📜 README.md         # Project documentation
```

---

## 🚀 How to Run

1. **Clone the repository**:

   ```bash
   git clone https://github.com/yourusername/IVA_Lab_2.git
   cd IVA_Lab_2
   ```

2. **Install Dependencies**:

   ```bash
   pip install opencv-python
   ```

3. **Run the Notebook**:
   Open `IVA_LAB_2.ipynb` in Jupyter Notebook or JupyterLab and run all the cells. Make sure your webcam is connected and accessible.

---

## 🔍 Implementation Overview

1. **Load Haar Cascade Classifiers**:

   ```python
   face_cascade = cv2.CascadeClassifier('haarcascade_frontalface_default.xml')
   eye_cascade = cv2.CascadeClassifier('haarcascade_eye.xml')
   ```

2. **Access Webcam Stream**:

   ```python
   cap = cv2.VideoCapture(0)
   ```

3. **Process Each Frame**:

   * Convert to grayscale
   * Detect faces and draw rectangles
   * Within each detected face, detect eyes
   * Display live results

4. **Terminate on Keypress**:
   Press `Esc` or `q` to stop the video stream.

---

## 🧪 Output

* Real-time video feed with:

  * Green rectangles around detected faces
  * Blue rectangles around detected eyes

---

## 💡 Applications

* Face detection in surveillance systems
* Emotion analysis and face tracking
* Access control using facial verification
* Smart mirrors, kiosks, and camera systems

---

## 📝 Notes

* Ensure the Haar cascade `.xml` files are in the correct path
* Lighting and camera quality can affect detection accuracy
* For better results, you may explore DNN-based models or `dlib`


