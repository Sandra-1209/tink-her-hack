# tink-her-hack

Project Description
The Smart Blind Stick is an Arduino-based assistive device developed to enhance the safety of visually impaired individuals. It uses an ultrasonic sensor to detect obstacles, a water sensor to identify wet surfaces, and an MPU6050 accelerometer to detect falls. When a hazard is detected, the system activates a buzzer and vibration motor to alert the user, and a push button is provided to reset the system after a fall alert. The device operates without GSM or GPS, making it a low-cost, efficient, and reliable safety solution for daily use.

| Sl. No | Component Name            | Quantity | Total Cost (INR) | Description                                |
| ------ | ------------------------- | -------- | ---------------- | ------------------------------------------ |
| 1      | Arduino Uno              | 1        | ₹400             | Main microcontroller unit                  |
| 2      | MPU6050 Module            | 1        | ₹150             | Accelerometer & gyroscope (Fall detection) |
| 3      | HC-SR04 Ultrasonic Sensor | 1        | ₹100             | Obstacle detection                         |
| 4      | Water Sensor Module       | 1        | ₹80              | Water detection                            |
| 5      | Active Buzzer             | 1        | ₹30              | Audio alert                                |
| 6      | Coin Vibration Motor      | 1        | ₹60              | Vibration alert                            |
| 7      | Jumper Wires (Set)        | 1        | ₹80              | Electrical connections                     |
| 8      | Breadboard                | 1        | ₹100             | Circuit assembly                           |
| 9      | 9V Battery + Connector    | 1        | ₹70              | Power supply                               |


Final total cost 1070

Assembly Instructions
Step 1: Prepare Components
Collect all components:Arduino uno,MPU6050,HC-SR04,Water Sensor,Active Buzzer,Coin Vibration Motor,Breadboard,Jumper Wires 
Ensure Arduino IDE and required libraries (Wire, MPU6050) are installed.

Step 2: Mount the Arduino
Place the Arduino Uno.
Do not power it yet

Step 3: Connect the MPU6050 (Fall Detection)
MPU6050 Pin-Arduino Nano
VCC-5V
GND-GND
SDA-A4
SCL-A5
This enables I2C communication.

Step 4: Connect the Ultrasonic Sensor
HC-SR04 Pin-Arduino uno
VCC-5V
GND-GND
Trig-D2
Echo-D3
Mount the ultrasonic sensor facing forward

Step 5: Connect the Water Sensor
Water Sensor-Arduino
VCC-5V
GND-GND
A0-A0
Fix the sensor near the bottom end of the stick.

Step 6: Connect the Buzzer
+-D8
–GND
This provides audio alert.

Step 7: Connect the Vibration Motor
Motor Wire
Positive-D9
Negative-GND
This provides tactile feedback.

Step 8: Power Connections
Connect 9V battery to VIN and GND of Arduino.
Ensure polarity is correct.
Double-check all GND connections are common.

Step 9: Upload the Program
Connect Arduino to laptop via USB.
Open Arduino IDE.
Select correct board (Nano).
Select correct COM port.
Upload the Smart Blind Stick code.
Open Serial Monitor to verify MPU6050 connection.

tep 10: Testing

Obstacle Test
Place object within 50 cm → Alert should activate.

Water Test
Touch water sensor with wet finger → Alert should activate.

Fall Test
Shake the device strongly and keep still → Continuous alarm should activate

Setup Guide
1. Software Setup
Install Arduino IDE
Download and install Arduino IDE on your laptop.
Open the software after installation.

Install Required Library
Go to Sketch → Include Library → Manage Libraries
Search for “MPU6050”
Install the required MPU6050 library.
Make sure the Wire library is available 

2. Hardware Setup
Place Arduino Uno
Insert Arduino Uno properly.

Connect All Sensors
Connect MPU6050 using I2C (A4 → SDA, A5 → SCL).
Connect Ultrasonic sensor to D2 (Trig) and D3 (Echo).
Connect Water sensor to A0.
Connect Buzzer to D8.
Connect Vibration motor to D9.
Make sure all GND pins are connected together.

3. Power Setup
Use USB cable during testing.
After testing, connect 9V battery to VIN and GND.
Ensure correct polarity.
Do not power both USB and battery simultaneously (unless required).

4. Code Upload Setup
Connect Arduino to laptop via USB.
Open your project code.
Go to Tools → Board → Arduino Nano.
Select correct Processor (Old Bootloader if needed).
Select correct COM Port.
Click Upload.
Wait for “Done Uploading”

5. Initial Testing
 Check MPU6050
Open Serial Monitor.
If connected properly, no error message appears.

Check Obstacle Detection
Place object in front of ultrasonic sensor.

 Check Water Detection
Touch water sensor with wet finger.

 Check Fall Detection
Shake device strongly and keep still.

6. Final Mounting
Fix ultrasonic sensor at front.
Place water sensor at bottom.
Secure Arduino and modules inside protective casing.
Arrange wires neatly to avoid short circuits

Team members
Nandana Sankar and Sandra S

Licensed under MIT License


