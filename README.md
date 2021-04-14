# CS207-Project Arduino Sonar

This project for CS207 uses a HC-SR04 Ultrasonic sensor to find range of objects in its path.

This Ultrasonic distance sensor has two ultrasonic transducers. One acts as a transmitter which converts electrical signal into 40 KHz ultrasonic sound pulses and the other listens for these transmitted sound wave to find the distance the wave travelled. It is combined with a servo motor to get distance of objects at various angle to replicate
a real sonar. It also warns the owner with a LED and a speaker when something is near it.


# Materials Used

Arduino UNO
HC-SR04 Utrasonic Range Finder
HXT 900 Servo motor
Jumper Wires
LED
A Piezo Speaker
A 560 ohm resistor
# Dependencies
Arduino NewPing Library https://www.arduino.cc/reference/en/libraries/newping/
Arduino TimerFreeTone Library https://forum.arduino.cc/t/timerfreetone-library-v1-5-play-tones-without-timers-and-therefore-no-conflicts/229448


# Build Instructions

To find distances at different angles I connected the servo motor to the Ultrasonic sensor both of which are connected to the breadboard via jumper wires. A LED and
a Piezo speaker were also connected later. Yellow wires are used to connect to the PINs while Red indicates connectin to +5V and Blue/Black wires are used to connect
to Ground. A fritzing diagram and a breadboard image is included in this repository.

Update:In the diagrams and images the sensor is connected directly to the breadboard because the servo motor has stopped working and I do not have enough time to get
a new one.

# Usage

After uploading the code to arduino it calculates the angle and the distance between the objects in cm and print it to the console. The LED remains OFF until a object 
is within 15cm of the sensors range and the speaker turns ON when it is within 10cm of range.

# Team
Navkiratpaul Singh

# Credits
Tony ZHANG https://create.arduino.cc/projecthub/faweiz/arduino-radar-69b8fe
