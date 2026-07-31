🚆 *Smart-Railway-Wildlife-Protection-System*

Overview

The Smart Railway Wildlife Protection System is an Arduino-based safety project designed to help reduce wildlife accidents near railway tracks. The system uses an ultrasonic sensor to detect the presence of an object (representing an animal) near the railway track. When an object is detected within the predefined distance, the system automatically activates warning signals, lowers a railway barrier using a servo motor, and displays an alert message on an OLED display.

This project demonstrates how embedded systems and sensors can be used to improve railway safety through early detection and automated warnings.

---

Features

- Animal detection using an HC-SR04 Ultrasonic Sensor
- Automatic railway warning system
- Servo motor-operated railway barrier
- Red and Green railway signal LEDs
- Active buzzer for audible alerts
- OLED display showing system status
- Detection counter displayed on screen
- Low-cost and beginner-friendly Arduino project

---

Components Used

- Arduino Uno R3
- HC-SR04 Ultrasonic Sensor
- SG90 Servo Motor
- 0.96-inch OLED Display (I2C)
- Active Buzzer
- Red LED
- Green LED
- Two 220Ω Resistors
- Breadboard
- Jumper Wires
- USB Cable
- 5V Power Supply
- Toy Railway Track (Prototype)
- Toy Train (Prototype)

---

Working Principle

1. The ultrasonic sensor continuously measures the distance in front of the railway track.
2. If an object is detected within approximately 20 cm, the Arduino interprets it as an animal on the track.
3. The system automatically:
   - Turns ON the red warning LED.
   - Turns OFF the green LED.
   - Activates the buzzer.
   - Lowers the railway barrier using the servo motor.
   - Displays "ANIMAL DETECTED - STOP TRAIN" on the OLED display.
4. When the object moves away, the system:
   - Turns ON the green LED.
   - Turns OFF the red LED.
   - Stops the buzzer.
   - Opens the railway barrier.
   - Displays "SYSTEM READY - SAFE".

---

Pin Connections

Component| Arduino Pin
HC-SR04 TRIG| D2
HC-SR04 ECHO| D3
Servo Motor| D5
Active Buzzer| D6
Green LED| D7
Red LED| D8
OLED SDA| A4
OLED SCL| A5
All VCC| 5V
All GND| GND

---

Folder Structure

Smart-Railway-Wildlife-Protection-System/
│
├── README.md
├── Smart_Railway_Wildlife_Protection_System.ino
├── Circuit_Diagram.png
├── BOM.csv
├── Project_Report.pdf
├── Journal.pdf
│
├── Photos/
│   ├── Photo1_Components.jpg
│   ├── Photo2_Circuit.jpg
│   ├── Photo3_Prototype.jpg
│   ├── Photo4_Detection.jpg
│   └── Photo5_Final.jpg
│
└── Demo/
    └── Demo_Video.mp4

---

Applications

- Railway safety demonstrations
- Wildlife conservation awareness
- Smart transportation projects
- School and college science exhibitions
- Arduino and embedded systems learning

---

Advantages

- Low-cost prototype
- Easy to build and understand
- Automatic detection and warning
- Demonstrates embedded systems concepts
- Expandable for future improvements

---

Future Improvements

- Replace the ultrasonic sensor with thermal or AI-based vision for improved wildlife detection.
- Add GSM or Wi-Fi alerts to notify railway authorities.
- Include GPS to report the location of detections.
- Record detections on an SD card or cloud platform.
- Integrate solar power for remote installations.

---

Safety Note

This prototype is an educational model intended to demonstrate automatic detection and warning concepts. It is not intended for deployment on real railway lines without extensive engineering, testing, and approval by railway authorities.

---

Author

Prince Kumar

- Hack Club Participant
- Learning Advanced Python, HTML, CSS, JavaScript, C++, and Java
- Interested in Embedded Systems, Robotics, Mathematics, and Open Source Projects

---

License

This project is released under the MIT License.

You are free to use, modify, and share this project for educational purposes with appropriate credit to the original author.