# 🏋️‍♂️ Real-Time Exercise Tracker and Counter

This project is a real-time computer vision application that tracks human body movements to count **push-ups**, **squats**, and **reps** using **MediaPipe**, **OpenCV**, and **Python**. It also includes a web app version built with **Flask** and **HTML** to combine all exercise counters in a unified interface.

---

## 🔍 Features

- ✅ Real-time pose detection using MediaPipe  
- 🔢 Push-up and squat counter based on joint angles  
- 📐 Angle calculation using landmark positions  
- 📊 Live feedback on movement stages and count  
- 🌐 Flask + HTML-based web interface for app version  
- 📦 Modular structure to easily expand to more exercises  

---

## 🧠 How It Works

- **MediaPipe** detects 33 pose landmarks on the body.
- The **angle between key joints** (like shoulder, elbow, and wrist) is calculated.
- Based on the **average angle of both arms or legs**, the stage ("up"/"down") is determined.
- **Counters are incremented** when a full rep is completed.
- Visual feedback (angle, stage, count) is rendered on the live camera feed.

---

## 📸 Sample Output



```bash
+-------------------------+
| PUSHUPS:        5      |
| STAGE:         UP      |
+-------------------------+
```

---

## 🚀 Getting Started

### 📦 Requirements

- Python 3.7+
- OpenCV
- MediaPipe
- NumPy
- Flask (for web version)

### 🔧 Installation

Clone the repository and install dependencies:

```bash
git clone https://github.com/manoj-naga-varma/Real-Time-Exercise-Tracker-and-Counter-in-Python.git
cd Real-Time-Exercise-Tracker-and-Counter-in-Python
pip install -r requirements.txt
```

---

### 🏃 Run the Push-up Tracker

```bash

python Pushups.py

```

---

### 🌐 Run the Flask Web App

```bash
cd app
python app.py
```

Then open your browser and go to:  
[http://localhost:5000](http://localhost:5000)

---

## 📁 Project Structure

```bash
exercise-tracker/
│
├── pushup_counter.py        # Real-time push-up counter logic
├── squat_counter.py         # Real-time squat counter logic
├── rep_counter.py           # Repetition counter logic
├── app/
│   ├── app.py               # Flask backend
│   ├── templates/
│   │   └── index.html       # HTML frontend
├── README.md                # Project documentation
└── requirements.txt         # Python dependencies
```


---

## 🤝 Contributing

Pull requests are welcome! If you find bugs or want to add new features (e.g., more exercises, dashboard, API), feel free to contribute.

---


---
