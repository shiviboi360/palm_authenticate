# Palm Registration & Verification System 🖐️

This project allows users to register their left and right palm prints and later verify identity using a trained CNN model.

## Features
- Register with webcam (left and right palm)
- Verify via webcam or image upload
- Auto-detect identity using saved model
- Tkinter GUI for interaction

## Requirements
- TensorFlow
- Keras
- OpenCV
- PIL
- NumPy

## Additional Setup
- A CNN model is trained and saved as `palm_model.h5` within the code itself during initial execution.
- A `register/` directory must exist (or will be created) to store user palm images.
- Palm images must follow the naming format: `###_S_L.jpg` and `###_S_R.jpg` (`###` = user ID like 001, 002...).
- Images are resized to 227x227 during processing.
- The label (ID) is auto-generated sequentially based on existing folders in `register/`.

## How to Run
1. Launch the app using the main Python file.
2. Use the GUI to:
   - Capture palm images for new registration.
   - Upload or capture a palm image to verify.
   - Unregister users by their label ID.

## Note
- The model must be trained using the same image naming convention and structure used during registration.
- The system supports verification even if only one hand is used during prediction.
