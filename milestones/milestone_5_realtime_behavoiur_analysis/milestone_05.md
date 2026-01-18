## 🔵 Milestone 5: Real-Time Behavior Classification (ANN)

### 📌 Objective
To classify human behavior in real-time as **Normal, Suspicious, or Dangerous**
by combining pose-based motion features with an Artificial Neural Network.

This milestone represents the **decision-making brain** of the system.

---

### 🧠 How It Works
- Pose landmarks are detected from video frames
- Motion features are extracted:
  - Arm angle (posture)
  - Hand speed (movement intensity)
- Features are fed into a trained ANN model
- Behavior prediction is generated per frame
- Result is overlaid directly on video output

---

### 🏗️ Model Details
- Framework: TensorFlow / Keras
- Model Type: Artificial Neural Network (ANN)

```text
Input Layer (2 features)
↓
Dense Layer (16 neurons, ReLU)
↓
Dense Layer (8 neurons, ReLU)
↓
Output Layer (3 neurons, Softmax)
