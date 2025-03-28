![Alt Text](https://github.com/meghawadhwani20/Hand-Gesture-LEDs-using-Arduino/blob/main/img1.jpg)

# Hand Gesture Controlled LED System

##  Project Overview
This project allows users to control LEDs using hand gestures, leveraging OpenCV for gesture recognition and PyFirmata for Arduino communication. The system detects specific finger positions and turns LEDs on or off accordingly.

##  Technologies Used
- **Python** (for gesture detection and Arduino communication)
- **OpenCV** (for hand tracking)
- **Mediapipe** (for finger detection)
- **PyFirmata** (for interfacing with Arduino)
- **Arduino** (as the LED controller)

##  Project Structure
```
├── new.py          # Main script for hand gesture detection
├── controller.py   # Arduino communication and LED control
├── README.md       # Project documentation
```

##  Hardware Requirements
- Arduino board (e.g., Uno, Mega)
- LEDs (at least 5)
- Resistors (220Ω for each LED)
- USB cable for Arduino
- Computer with Python installed

##  Installation Steps
1. Clone this repository:
   ```bash
   git clone https://github.com/your-repo/hand-gesture-led.git
   cd hand-gesture-led
   ```
2. Install required dependencies:
   ```bash
   pip install opencv-python mediapipe pyfirmata
   ```
3. Connect the Arduino to your computer and note the COM port (e.g., `COM12` or `/dev/ttyUSB0`). Update `controller.py` accordingly.

##  How to Run
1. Upload the **StandardFirmata** firmware to your Arduino via the Arduino IDE.
2. Run the gesture detection script:
   ```bash
   python new.py
   ```
3. The system will recognize hand gestures and control LEDs accordingly.

##  Gesture-to-LED Mapping
- ✊ **All fingers down** → All LEDs OFF
- ☝ **Index up** → LED 1 ON
- ✌ **Index & Middle up** → LED 1 & 2 ON
- 🤟 **Index, Middle & Ring up** → LED 1, 2 & 3 ON
- 🖐 **All fingers up** → All LEDs ON

##  Future Enhancements
- Add more complex gesture recognition
- Implement voice control as an additional feature
- Enhance the UI for better interaction

## Video Link:https://www.linkedin.com/feed/update/urn:li:activity:7293503781948776448/




