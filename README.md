# 🖐️ Palm Registration & Verification System

This project enables biometric registration and identity verification using palm prints. Users can register their left and right palm images via webcam, and later verify their identity using either a live capture or an uploaded image. The system uses a trained CNN model to predict identity and is built with a Tkinter GUI.

---

## 🚀 Project Overview

Palm-based biometrics are gaining traction in secure authentication systems due to their uniqueness and ease of acquisition. This application offers a local, privacy-conscious solution to palm print registration and verification, ideal for research, prototypes, or edge-device authentication.

---

## 🧠 Features

- 📸 Live Webcam Capture (left & right palm)
- 🧠 CNN-based Identity Prediction
- 🖼️ Upload or live image for verification
- 🧹 User unregistration with one click
- 🪟 Tkinter GUI interface for ease of use

---

## 🔐 Applications

This project is suitable for:

- Aadhaar-style government enrollment
- Border control and immigration checkpoints
- Contactless attendance in hospitals or offices
- Access control in secure labs or bank vaults

---

## 📦 Requirements

Ensure the following Python libraries are installed:

- TensorFlow
- Keras
- OpenCV
- PIL (Pillow)
- NumPy

Install them via:

```bash
pip install tensorflow keras opencv-python pillow numpy
```

---

## ⚙️ Setup & Structure

- CNN model is trained and saved as `palm_model.h5` during first execution.
- A `register/` folder is created to store user palm images.
- Naming format:
  - `###_S_L.jpg` – Left palm
  - `###_S_R.jpg` – Right palm
  - `###` is a user ID like 001, 002, etc.
- All images auto-resized to `227x227` pixels.

---

## ▶️ How to Run

1. Launch the app:
   ```bash
   python main.py
   ```

2. Use the GUI:
   - 🖐️ Register new users
   - 📤 Upload or capture palm image for verification
   - 🗑️ Unregister a user by ID

---

## 📄 License

This project is licensed under the MIT License.
