# Milestone 4: Pose Detection & Motion Feature Extraction

## 📌 Objective

The objective of this milestone is to detect human body pose from video
and extract **motion-based numerical features** required for behavior analysis.

This milestone bridges **raw video input** and **ML-based behavior classification**.

---

## 🧠 Problem Solved

Object detection alone is insufficient to understand intent.
Pose-based motion analysis enables understanding:

- Body posture
- Arm movement
- Motion intensity

These signals are critical for intelligent surveillance systems.

---

## 🎥 Input

- Video footage (`pose_detection_demo.mp4`)
- Single-person visible in frame

---

## 🧩 Technologies Used

- Python
- OpenCV
- MediaPipe Pose
- Google Colab (for visualization)

---

## 🏗️ Pipeline Overview

```text
Video
 ↓
Frame Extraction
 ↓
RGB Conversion
 ↓
Pose Landmark Detection
 ↓
Skeleton Visualization
 ↓
Motion Feature Extraction



## 📍 Pose Landmarks Used

RIGHT_SHOULDER

RIGHT_WRIST

These landmarks are used to compute arm posture and motion.

```

## 📊 Extracted Features

Feature Description
Arm Angle Vertical displacement between shoulder and wrist
Hand Speed Frame-to-frame wrist movement

## 🧪 Sample Output

Frame read: True
Arm Angle: 108.34
Hand Speed: 0.0321

## Visualization

Skeleton overlay on person

5 sample frames displayed per run (Colab-safe)

Real-time feature values printed per frame

## ✅ Results

✔️ Video frames successfully read
✔️ Pose detected reliably
✔️ Skeleton drawn on person
✔️ Numerical motion features extracted

## 🚀 Real-World Application

This milestone enables:

Suspicious activity analysis

Gesture-based threat detection

Input preparation for ML classifiers
