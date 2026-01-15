# Milestone 2: Human Pose & Movement Analysis

## 📌 Objective

The objective of this milestone is to analyze **human posture and hand movement**
from video footage to understand **behavior patterns**, not just object presence.

This step is crucial because:

- Holding an object does not always mean a threat
- Behavior and movement decide intent

---

## 🧠 What This Module Does

- Detects full human body pose from video
- Extracts key body landmarks (shoulder, elbow, wrist)
- Calculates arm angles
- Measures hand movement speed over time
- Converts visual movement into numerical features

---

## 🛠️ Technologies Used

- Python
- MediaPipe Pose
- OpenCV
- NumPy
- Google Colab

---

## 📂 Input

- Video footage (`.mp4`)
- Single or multiple persons in frame

---

## 📊 Features Extracted

| Feature Name   | Description                              |
| -------------- | ---------------------------------------- |
| Arm Angle      | Measures posture (relaxed vs aggressive) |
| Hand Speed     | Measures movement intensity              |
| Wrist Position | Used for motion tracking                 |

These features will be used in the next milestone
for **ANN-based behavior classification**.

---

## 🎥 Sample Output

- Pose skeleton drawn on the person
- Numerical values printed for:
  - Arm angle
  - Average hand movement speed

---

## 🚀 Use Case

This module helps differentiate between:

- Normal activities (e.g., vendor holding knife)
- Suspicious behavior
- Potential public threats

---

## 📈 Status

✅ Completed successfully  
✅ Features saved for ANN training
