# mask_detection_vending_machine-main

[![Language](https://img.shields.io/badge/Language-Python-yellow.svg?style=for-the-badge)](https://en.wikipedia.org/wiki/Programming_language)

This project combines **real-time facial mask detection** with a potential **vending machine automation system**. Using computer vision and deep learning, the system detects whether a user is wearing a mask and can be extended to automate dispensing actions—such as granting or denying access to services based on detection results.

---

## 📚 Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)

---

## 🚀 Features

Based on the project structure, the following functionalities are included or intended:

- **Real-Time Mask Detection**:
  - Uses webcam or video input to detect faces and identify whether a person is wearing a mask.

- **Trained Deep Learning Model**:
  - Utilizes a pre-trained Keras model (`mask_detector.model`) to perform classification.

- **Face Detection Module**:
  - Employs OpenCV and pre-trained face detection models located in the `face_detector` directory (possibly `.caffemodel` or `.prototxt` files).

- **User Interface**:
  - A GUI interface (`project_ui.py`) that might simulate a vending machine interface for interaction and access control.

- **Modular Execution Scripts**:
  - Includes multiple scripts such as `main_run.py`, `main.py`, and `detect_mask_video.py` that likely provide different functionalities (e.g., raw detection, UI integration, testing).

---

## 🧰 Technologies Used

- **Python** (Primary language)
- **TensorFlow / Keras** (Model loading and inference)
- **OpenCV** (Video stream processing and face detection)
- **Imutils** (Image processing utilities)
- **NumPy** (Numerical operations)

> ⚠️ Refer to `requirements.txt` or install common packages below.

---

## ⚙️ Installation

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/mask_detection_vending_machine-main.git
   cd mask_detection_vending_machine-main
   ```

2. **(Optional) Create and Activate a Virtual Environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install Required Dependencies**
   Install the core libraries for detection:
   ```bash
   pip install opencv-python tensorflow keras imutils numpy
   ```
   Or install from the `requirements.txt` file (if available):
   ```bash
   pip install -r requirements.txt
   ```

---

## ▶️ Usage

Several scripts are available for different use cases. Start with the one that fits your workflow:

### 🧪 Run Video-Based Mask Detection
```bash
python detect_mask_video.py
```

### 🧩 Run Main Program (possibly linked to vending logic)
```bash
python main_run.py
```

### 🖥️ Run UI Interface
```bash
python project_ui.py
```

> 📌 Before running:
> - Ensure your webcam is connected and accessible.
> - Make sure the files `mask_detector.model` and the `face_detector` directory are present.

---

## 📂 Project Structure

```bash
├── mask_detector.model              # Trained mask detection model
├── face_detector/                   # Contains face detection models (deploy.prototxt, res10_300x300_ssd.caffemodel)
├── detect_mask_video.py             # Real-time video mask detection script
├── main_run.py                      # main control logic
├── main.py                          # Alternate main script
├── project_ui.py                    # User interface for vending machine
├── requirements.txt                 # Python dependencies
└── README.md                        # Project documentation
```

---

## 🤝 Contributing

We welcome contributions to improve or extend this system!

1. Fork the repository  
2. Create your feature branch:
   ```bash
   git checkout -b feature/AmazingFeature
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add AmazingFeature"
   ```
4. Push to your branch:
   ```bash
   git push origin feature/AmazingFeature
   ```
5. Open a pull request for review.

---
