# 🧠 Milestone 3: ANN-Based Human Behavior Classification

## 📌 Overview

This milestone focuses on classifying human behavior into
Normal, Suspicious, or Dangerous using an Artificial Neural Network (ANN).

It adds decision-making intelligence on top of object detection and pose estimation developed in previous milestones.

## 🎯 Objective

The goal of this milestone is to:

Analyze human movement patterns

Convert them into numerical features

Use an ANN to predict behavior intent

This allows the system to move beyond what object is detected to how the person is behaving.

## 🧠 Problem Statement

Object detection alone cannot answer critical questions like:

Is a person behaving aggressively?

Is rapid movement a potential threat?

Is the situation normal or dangerous?

This milestone solves that gap by introducing behavior classification using machine learning.

## 🔄 Pipeline Flow

Video Input
↓
Pose Estimation (Milestone 2)
↓
Feature Extraction
↓
ANN-Based Classification
↓
Behavior Output (Normal / Suspicious / Dangerous)

## 📊 Input Features

The ANN model is trained using numerical features derived from pose data.

Feature Name Description
Arm Angle Represents posture (relaxed vs aggressive stance)
Hand Speed Measures motion intensity (slow vs rapid movement)

📌 These features are extracted during Milestone 2 (Pose Detection).

## 🏗️ Model Architecture

Framework: TensorFlow / Keras

Model Type: Artificial Neural Network (ANN)

Input Layer (2 Features)
↓
Dense Layer (16 Neurons, ReLU)
↓
Dense Layer (8 Neurons, ReLU)
↓
Output Layer (3 Neurons, Softmax)

## 🎯 Output Classes

Class Index Behavior Type
0 Normal Behavior
1 Suspicious Behavior
2 Dangerous Behavior
🔍 Training Details

Feature Scaling: MinMaxScaler

Learning Type: Supervised Learning

Loss Function: Sparse Categorical Crossentropy

Optimizer: Adam

Evaluation Metric: Accuracy

The model was trained on labeled movement data representing different behavioral patterns.

## ✅ Results & Validation

The ANN successfully classifies human behavior based on movement intensity and posture.

🔎 Example Prediction
test_sample = np.array([[110, 0.35]]) # Raised arm + fast movement
prediction = model.predict(test_sample)
print("Predicted class:", np.argmax(prediction))

Output:

Predicted class: 2

## 📌 Interpretation:

The model correctly identifies the behavior as Dangerous.

🎥 Testing & Demonstration

A testing video demonstrating real-time pose detection and behavior classification is included in this milestone.

## 📂 Location:

/testing_videos/

## 🎯 Purpose:

Helps interviewers visually understand the system

Shows real-world execution

Demonstrates model effectiveness beyond theory

## 🚀 Real-World Applications

This milestone enables:

Intelligent CCTV surveillance systems

Automated threat detection

Real-time alert generation

Smart city security infrastructure

Foundation for law enforcement analytics

## 📈 Current Status

✅ Milestone 3 Completed
✅ ANN Model Trained & Tested
✅ Behavior Classification Working
✅ Ready for Integration with Alert System

## 🔜 Next Steps (Upcoming)

Integrate behavior output with alert/notification system

Combine object type + behavior for risk scoring

Optimize for real-time deployment

Deploy on edge devices or cloud
