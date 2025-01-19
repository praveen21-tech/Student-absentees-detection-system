# Student-absentees-detection-system
# Student Absentees Detection System

This repository contains a Python-based system for detecting student attendance using face recognition from CCTV or webcam video feeds. The system uses real-time face detection and recognition to identify students and mark their attendance in a CSV file.

---

## Features

- **Real-Time Face Recognition**: Detect and recognize student faces from video streams.
- **Attendance Logging**: Automatically logs attendance in a CSV file with timestamps.
- **Support for Preloaded Student Data**: Load student images as known faces for recognition.
- **Customizable Video Source**: Works with both live webcam feeds and pre-recorded video files.

---

## Prerequisites

- **Python 3.7 or above**
- Libraries:
  - `opencv-python`
  - `face-recognition`
  - `numpy`
  - `datetime`

Install the required libraries:
```bash
pip install opencv-python face-recognition numpy
```

---

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/student-absentees-detection.git
   cd student-absentees-detection
   ```

2. Prepare a folder with student images:
   - Place the images of each student in a folder, e.g., `students_images/`.
   - Name each image file as the student’s name (e.g., `Alice_Johnson.jpg`).

3. Ensure the required files are present:
   - **Video Source**: Provide a video file (e.g., `simulated_cctv.mp4`) or use a webcam.
   - **Background** (optional): Use a static background image for simulation.

---

## Usage

1. Run the script:
   ```bash
   python attendance_detection.py
   ```

2. **Video Feed**:
   - The script will display the video feed with detected faces labeled by name.

3. **Attendance Log**:
   - Attendance is saved in `attendance.csv` with the following format:
     ```csv
     Name,Timestamp
     Alice Johnson,2025-01-06 14:05:23
     Bob Smith,2025-01-06 14:06:12
     ```

---

## Code Structure

```
student-absentees-detection/
├── attendance_detection.py   # Main script for detection
├── students_images/          # Folder containing student images
├── untiled_project_V2.mp4        # Optional video source for testing
├── attendance.csv            # Output attendance file
└── README.md                 # Project documentation
```

---

## Customization

- **Video Input**:
  - Change the `cv2.VideoCapture` parameter to `0` for webcam or provide a video file path.

- **Attendance File**:
  - Modify the `ATTENDANCE_FILE` variable in the script to change the output file name or location.

- **Face Encoding**:
  - Add or update student images in the `students_images` folder and rerun the script to refresh encodings.

---

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## Contributing

Contributions are welcome! Please fork this repository and submit a pull request for any features or improvements.

---

## Acknowledgments

- Built with the [face_recognition](https://github.com/ageitgey/face_recognition) library.
- Inspired by real-world applications in education and security systems.

---

## Contact

For questions or support, contact [praveen2006offical@gmail.com](mailto:praveen2006offical@gmail.com).

