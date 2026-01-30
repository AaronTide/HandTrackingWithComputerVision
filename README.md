
# 🎨 AI Virtual Painter — Draw in the Air With Computer Vision

## ✨ Story & Motivation

I’ve always wanted to be an **online educator** — someone who can explain ideas visually, not just with words.
While teaching (and learning) online, I noticed a gap: **drawing naturally in the air**, the way teachers do on a physical board, is still awkward with a mouse or stylus.

So I built this **AI- Powered Air Canvas**.

This project lets you **draw on a virtual canvas using just your hand**, tracked in real time by state of the art AI models through a webcam. No touchscreen. No stylus. Just intuitive hand gestures.

The goal wasn’t just to build a cool computer vision demo —
it was to create a **teaching-friendly, interactive tool** that makes explanations more natural, visual, and engaging.

---

## 🚀 What is Air Canvas?

**Air Canvas** is a real-time computer vision application that allows you to:

* ✋ Track your hand using a webcam
* ✍️ Draw in the air with your index finger
* 🎨 Switch colors using hand gestures
* 🧠 Use gesture logic (fingers up/down) to control drawing
* 🖥️ See everything live on a virtual canvas

It’s inspired by the idea of turning **human gestures into digital interaction** — especially for education, presentations, and creative expression.

---

## 🛠️ Tech Stack

* **Python 3.11**
* **OpenCV** — webcam input, drawing, UI
* **MediaPipe (0.10.29)** — real-time hand landmark detection
* **NumPy** — array & image operations

---

## 📁 Project Structure

```
Air-Canvas/
│
├── HandTrackingModule.py     # Reusable hand detection + gesture logic
├── VirtualPainter.py         # Main Air Canvas application
├── Header                    # Project image headers
└── README.md                # Project documentation
```

---

## ✋ How It Works 

1. **Webcam captures frames**
2. **MediaPipe detects 21 hand landmarks**
3. Finger states are inferred using landmark positions
4. Gesture logic determines:

   * When to draw
   * When to switch colors
   * When to clear canvas
5. OpenCV overlays drawings in real time

This modular approach makes the system **easy to extend** for:

* Gesture-based controls
* Teaching tools
* Interactive whiteboards

---

## ⚙️ Setup Instructions

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/AaronTide/AI_Virtual_Painter_With_ComputerVision.git
cd AI_Virtual_Painter_With_ComputerVision
```

---

### 2️⃣ Create a Virtual Environment

```bash
python -m venv .venv
```

Activate it:

**Windows**

```bash
.venv\Scripts\activate
```

**macOS / Linux**

```bash
source .venv/bin/activate
```

---

### 3️⃣ Install Dependencies

⚠️ **Important:** Must use Python 3.11 and these specific versions since newer Python versions are not yet supported by mediapipe.

Install compatible versions:

```bash
pip install numpy==1.26.4
pip install opencv-python
pip install mediapipe==0.10.29
```

---

### 4️⃣ Run the Application

```bash
python VirtualPainter.py
```

Make sure your webcam is connected and not in use by another app.

---

## 🖐️ Controls & Gestures

| Gesture                | Action         |
| ----------------       | -------------- |
| Index finger up        | Draw           |
| Two fingers up         | Select mode    |
| All fingers down       | Idle           |
| Use Eraser from header | Erase          |


*(Gesture logic can be customized in `HandTrackingModule.py`)*

---

## 🎓 Use Cases

* Online teaching & tutoring
* Explaining math, physics, or diagrams
* Interactive presentations
* Gesture-based UI experiments
* Computer vision learning projects

---

## 🌱 Future Improvements


* Save drawings as images
* Integrate with screen recording tools
* Convert to a web-based or tablet-friendly version

---

## 🤝 Why This Project Matters

This project sits at the intersection of:

* **Education**
* **Human–Computer Interaction**
* **Computer Vision**

Air Canvas is not just about drawing —
it’s about **making digital teaching more human**.

---

## 📌 Author

Built with curiosity and purpose by **Arifa Rahman**
Aspiring educator • Computer Vision enthusiast • Software Builder

---
Stars are my fuel, pls leave a star if you think this was cool <3
