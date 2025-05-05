🖐️ Palm Registration & Verification System

This project enables biometric registration and identity verification using palm prints. Users can register their left and right palm images via webcam, and later verify their identity using either a live capture or an uploaded image. The system uses a trained CNN model to predict identity and is built with a simple Tkinter-based GUI.

🚀 Project Overview

Palm-based biometrics are increasingly used in secure authentication systems due to their uniqueness and non-intrusiveness. This system offers a lightweight, local solution for palm print registration and verification — ideal for demos, research, and integration into larger security systems.

The application captures palm images, trains a Convolutional Neural Network (CNN) model, and allows for both verification and deregistration — all from a user-friendly Python GUI.

🧠 Features

- 📸 Live Webcam Capture for Left & Right Palm Registration
- 🔍 Verification via Live Feed or Image Upload
- 🧠 CNN-based Prediction Model for Identity Detection
- 💻 Tkinter GUI for Smooth User Interaction
- 🗃️ Auto-Organized Image Storage with Sequential ID Labeling

🔐 Applications

This system can be used in:

- Government ID Systems (e.g., Aadhaar-style enrollment)
- Immigration & Border Control for touchless identity verification
- Secure Facility Access (labs, banks, data centers)
- Healthcare/Attendance Systems for hygienic, contactless logging

📦 Requirements

Ensure the following Python libraries are installed:

- TensorFlow
- Keras
- OpenCV
- PIL (Pillow)
- NumPy

You can install them via:

pip install tensorflow keras opencv-python pillow numpy

⚙️ Setup & Structure

- The CNN model is automatically trained and saved as `palm_model.h5` during first-time execution.
- A `register/` directory will be created to store images.
- Palm images must follow this format:
  - ###_S_L.jpg → Left palm
  - ###_S_R.jpg → Right palm  
  (### is a sequential ID like 001, 002, etc.)
- All images are automatically resized to 227x227.

▶️ How to Run

1. Run the main Python script:
   python main.py

2. Use the GUI to:
   - 🖐️ Register new users (left and right palm)
   - 📤 Upload or live-capture for verification
   - 🗑️ Unregister a user by their ID label

📝 Notes

- During verification, even one palm (left or right) is sufficient for prediction.
- Ensure consistent lighting and hand positioning for better model accuracy.
- This is a local-only system and doesn’t store any biometric data in the cloud.

📄 License

This project is licensed under the MIT License.
