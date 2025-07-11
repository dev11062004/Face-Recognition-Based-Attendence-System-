# Face Recognition Attendance System

A modern, digital, and fully automated face recognition attendance system using Python, OpenCV, and scikit-learn.

## Features
- **Real-time Face Recognition** using your webcam
- **Attendance Logging** with timestamps in CSV files
- **Voice Feedback** for successful attendance
- **Digital, Customizable UI** with background image
- **Easy to add new faces** to the dataset

## How It Works
1. **Add Faces:**
   - Run `add_faces.py` to capture and store new faces with labels.
2. **Run Attendance:**
   - Run `test.py` to start the live face recognition and attendance logging.
   - Recognized faces are marked present in a dated CSV file in the `Attendance/` folder.
3. **Background Image:**
   - The UI uses `background.png` for a modern look. Replace it with your own image for customization.

## Project Structure
```
face_recognition_project-main/
├── add_faces.py           # Script to add new faces
├── app.py                 # (Optional) Main app logic
├── test.py                # Main attendance/recognition script
├── background.png         # UI background image
├── Attendance/            # Attendance CSV logs
├── data/                  # Face data, labels, and model files
│   ├── faces_data.pkl
│   ├── names.pkl
│   ├── haarcascade_frontalface_default.xml
│   └── ...
└── README.md              # Project documentation
```

## Requirements
- Python 3.7+
- OpenCV (`opencv-python`)
- scikit-learn
- numpy
- pywin32 (for Windows voice feedback)

Install dependencies:
```bash
pip install opencv-python scikit-learn numpy pywin32
```

## Usage
1. **Add new faces:**
   ```bash
   python add_faces.py
   ```
2. **Start attendance system:**
   ```bash
   python test.py
   ```
3. **View attendance:**
   - Check the `Attendance/` folder for daily CSV logs.

## Customization
- **Change UI background:** Replace `background.png` with your own image.
- **UI/UX:** The system overlays face boxes, names, and a digital clock on the video feed. You can further enhance the UI in `test.py`.

## Screenshots
*(Add your screenshots here)*

## License
This project is for educational purposes. Feel free to use and modify it for your needs.

---
**Made with Python, OpenCV, and scikit-learn.**
