# 🖱️ AI Virtual Mouse

This Python project allows users to control the mouse using hand gestures captured via a webcam. The system uses **OpenCV**, **MediaPipe**, and **PyAutoGUI** to track hand landmarks and translate specific gestures into mouse actions.

---

## 📌 Features

- 🖐️ Real-time hand gesture detection
- 🎯 Cursor movement with index finger
- 🖱️ Left click, Right click, Double click using hand gestures
- 📸 Take screenshots with a gesture

---

## 🛠️ Tech Stack

- Python 3.10
- OpenCV
- MediaPipe
- PyAutoGUI
- Pynput

---

## 📂 Project Structure

```
AI_Virtual_Mouse/
├── .venv310/               # Virtual environment (ignored in Git)
├── app/
│   └── app.py              # Main application script
├── requirements.txt        # Project dependencies
└── README.md               # Project documentation
```

---

## ⚙️ Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/your-username/AI_Virtual_Mouse.git
cd AI_Virtual_Mouse
```

### 2. Create and activate a virtual environment

```bash
py -3.10 -m venv .venv310
.venv310\Scripts\Activate.ps1   # For PowerShell
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ How to Run

```bash
python app/app.py
```

- Make sure your webcam is connected and enabled.
- Use gestures to move the mouse or perform clicks.

---

## 🤌 Gesture Mapping (Conditions)

| Action         | Gesture Condition                                            |
|----------------|--------------------------------------------------------------|
| **Move Mouse** | Thumb closed, Index finger upright                           |
| **Left Click** | Index finger bent, Thumb straight                            |
| **Right Click**| Thumb and Index straight, Middle finger bent                 |
| **Double Click**| Thumb straight, Index and Middle fingers bent               |
| **Screenshot** | All three (Thumb, Index, Middle) closed                      |

> 📸 Screenshots are saved as: `my_screenshot_<random>.png`


