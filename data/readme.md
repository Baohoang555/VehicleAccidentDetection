---

```markdown
# 🚗 AI-Driven Traffic Accident Detection System

> A real-time intelligent system for detecting traffic accidents from CCTV video streams using Deep Learning and Computer Vision.

---

## 📌 Overview

This project presents an end-to-end **AI-powered accident detection system** that analyzes traffic video streams to identify potential accidents in real-time.

The system combines:
- Object Detection (YOLOv8)
- Vehicle Tracking
- Motion & Behavior Analysis
- Deep Learning Classification

---

## 🧠 Key Features

✅ Real-time vehicle detection using YOLOv8  
✅ Multi-object tracking with unique vehicle IDs  
✅ Speed & trajectory estimation  
✅ Risk scoring for accident prediction  
✅ Accident classification (Accident / Non-Accident)  
✅ Visualization with bounding boxes and alerts  

---

## 🏗️ System Architecture

```

Video Input (CCTV)
↓
[ YOLOv8 Object Detection ]
↓
[ Vehicle Tracking System ]
↓
[ Motion Analysis ]
↓
[ Risk Scoring Algorithm ]
↓
[ Deep Learning Classifier ]
↓
🚨 Accident Alert Output

```

---

## 🛠️ Technologies Used

- Python
- OpenCV
- YOLOv8 (Ultralytics)
- TensorFlow / Keras
- NumPy
- Pandas
- Matplotlib / Seaborn

---

## 📂 Project Structure

```

├── data/                       # Dataset (Accident / NonAccident)
├── models/                     # Trained models
├── src/
│   ├── detection/              # YOLO detection
│   ├── tracking/               # Vehicle tracking logic
│   ├── analysis/               # Motion & risk analysis
│   ├── classification/         # Accident classifier
│   └── utils/                  # Helper functions
├── notebooks/                  # Experiments & training
├── main.py                     # Main pipeline
├── config.py                   # Configuration
└── README.md

````

---

## ⚙️ Installation

```bash
git clone https://github.com/Baohoang555/AI-Driven-Accident-Detection-System.git
cd AI-Driven-Accident-Detection-System
pip install -r requirements.txt
````

---

## ▶️ Usage

### Run the system:

```bash
python main.py
```

### Input:

* Video file OR webcam stream

### Output:

* Real-time detection with bounding boxes
* Accident alerts

---

## 📊 Dataset

* Source: Kaggle Traffic Accident Dataset
* Classes:

  * Accident
  * Non-Accident

---

## 📈 Model Performance

| Metric    | Value |
| --------- | ----- |
| Accuracy  | ~XX%  |
| Precision | ~XX%  |
| Recall    | ~XX%  |

*(Update after training)*

---

## 🚀 Future Improvements

* 🔹 Deploy with Streamlit (Web App)
* 🔹 Integrate real-time CCTV streams
* 🔹 Improve tracking with DeepSORT
* 🔹 Add alert notification system (SMS / Email)
* 🔹 Optimize for edge devices (Jetson Nano)

---

## 📸 Demo

*(Add screenshots or GIF here)*

---

## 🤝 Contributing

Contributions are welcome! Feel free to fork and submit pull requests.

---

## 📜 License

This project is licensed under the MIT License.

---

## 👨‍💻 Author

* Your Name

---

## ⭐ Acknowledgements

* Ultralytics YOLOv8
* Kaggle Dataset
* Open-source AI community

---