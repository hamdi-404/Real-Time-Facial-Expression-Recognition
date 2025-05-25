# 🧠 Real-Time Facial Expression Recognition

This project is a real-time facial expression recognition system that detects human emotions from facial images or live webcam input using deep learning techniques.

## 🎯 Objective
To build an accurate and efficient facial emotion recognition system trained on popular datasets using transfer learning and deployed in real-time.

## 📊 Datasets Used
The model was trained and evaluated on three widely-used datasets:
- **FER-2013**: Achieved 66% test accuracy
- **RAF-DB**: Achieved 82% test accuracy
- **AffectNet-7**: Achieved 72% test accuracy

Each dataset includes 7 facial expression classes:  
`Angry`, `Disgust`, `Fear`, `Happy`, `Sad`, `Surprise`, `Neutral`

## 🛠️ Techniques & Tools
- **Data Augmentation**: Rotation, zoom, brightness, horizontal flip, etc.
- **Transfer Learning**: Using `MobileNetV2` as base model
- **Progressive Fine-Tuning**:
  - Trained top layers with frozen MobileNetV2 (10 epochs)
  - Unfroze last 50 layers (5 epochs)
  - Unfroze last 75 layers (5 epochs)
  - Unfroze last 100 layers (5 epochs)
- **Libraries**: TensorFlow, Keras, OpenCV, NumPy

## 🧠 Model Architecture
- Base: MobileNetV2 (pretrained on ImageNet)
- Custom Head:
  - Global Average Pooling
  - Dense (128) + ReLU + Dropout (0.5)
  - Dense (128) + ReLU + Dropout (0.5)
  - Dense (7) with Softmax

## 🎥 Demo


## 📌 Requirements
- Python 3.8+
- TensorFlow 2.x
- OpenCV
- NumPy

## 📧 Contact
Made by **Hamdi** – Machine Learning Engineer 
**hamdi404.cs@gmail.com
For any questions, feel free to reach out or open an issue!

---

⭐ Star this repo if you found it useful!
