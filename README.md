# Color Detection with OpenCV (HSV Masking)

This project demonstrates real-time color detection using **OpenCV**, **HSV color space**, and **Pillow (PIL)**.  
The script captures frames from a webcam, applies a color mask, and draws a bounding box around the detected object.

---

## 📸 Features

- Real-time webcam color detection  
- HSV-based masking  
- Bounding box detection using PIL’s `getbbox()`  
- Press **q** to quit the stream

---

## 🧩 How It Works

1. Capture each frame from the webcam  
2. Convert the frame from **BGR → HSV**  
3. Compute HSV limits using `get_limits()` from `util.py`  
4. Create a mask with `cv2.inRange()`  
5. Use `mask.getbbox()` to find the detected region  
6. Draw a green rectangle around the detected color  
7. Display the processed video feed

---

## 🛠 Requirements

Install the required libraries:

```bash
pip install opencv-python pillow numpy
