# 🚗 Drowsiness Detector Using Python with SMS Alert

A real-time drowsiness detection system designed to enhance driver safety. This project uses Python, OpenCV, and Dlib to detect drowsiness, providing both an audio alert and an SMS notification for prompt action.

---

## 📝 Features

- **Real-Time Detection**: Monitors the driver’s face and eye movements via a webcam.
- **Eye Aspect Ratio (EAR) Calculation**: Detects drowsiness by analyzing eye closure patterns.
- **Audio Alerts**: Plays a warning sound when drowsiness is detected.
- **SMS Notifications**: Sends an SMS alert to a predefined contact using the Twilio API.
- **Facial Landmark Detection**: Utilizes Haar cascades and Dlib’s 68-point facial landmark predictor for precise detection.

---

## 📋 Requirements

### Ensure you have the following installed:

- Python 3.7 or higher
- Required Python Libraries:
  ```bash
  pip install numpy opencv-python pygame imutils scipy dlib twilio
### Dlib Shape Predictor Model:
- Download shape_predictor_68_face_landmarks.dat from Dlib's Model Zoo.
- Place the file in your project directory.

  ---

## ⚙️ Setup and Installation
### Clone the repository:
git clone https://github.com/your-username/Drowsiness-detector-using-python-with-sms-alert.git
cd Drowsiness-detector-using-python-with-sms-alert
### Install dependencies:
pip install -r requirements.txt
### Configure Twilio credentials:
Create a file named key.py in the project directory.
### Add the following:
account_sid = "your_account_sid"
auth_token = "your_auth_token"
twilio_number = "your_twilio_phone_number"
target_number = "target_phone_number"
Ensure the audio alert file (alert.wav) is in the project directory.

---

## 🚀 Usage
### Run the script:
python drowsiness_detection.py
The webcam will activate, and the system will start monitoring for drowsiness.

If drowsiness is detected:

An alert sound will play.
An SMS will be sent to the predefined number.
Press q to exit the application.

---

## 🛠️ How It Works
Eye Aspect Ratio (EAR):

EAR is calculated using the distances between specific eye landmarks.
If EAR falls below a set threshold for consecutive frames, the system detects drowsiness.
### Audio Alert:
The pygame library plays a warning sound to alert the driver.
### SMS Alert:
The Twilio API sends an SMS to notify others about the driver’s condition.

---

## 📂 File Structure

Drowsiness-detector-using-python-with-sms-alert/
│
├── alert.wav                      # Audio file for alert
├── drowsiness_detection.py        # Main script
├── shape_predictor_68_face_landmarks.dat # Dlib model for facial landmarks
├── key.py                         # Twilio credentials
├── requirements.txt               # Python dependencies
└── README.md                      # Project documentation

---

## 🧩 Future Enhancements
Add yawning detection for better accuracy.
Introduce a logging system to record drowsiness events with timestamps.
Optimize for mobile and edge devices.
Enhance the UI with more intuitive feedback mechanisms.

---

## 🛡️ License
This project is licensed under the MIT License. See the LICENSE file for details.

---

## 🤝 Contributing
Contributions are welcome! Feel free to open issues or submit pull requests to improve this project.

---

## 📬 Contact
### For inquiries or feedback, reach out to me:
Email: vivi420vishnu.com
GitHub: VichuA2







