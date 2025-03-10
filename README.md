# Clap_Activated_LED_System
A simple Arduino-based project that uses a KY-038 sound sensor to detect claps and toggle multiple LEDs on and off. This project demonstrates basic sound-activated control using a digital sound sensor and an Arduino Mega 2560. Ideal for beginners exploring sensor integration and real-time input processing.
Clap-Activated LED Control

🎤 Clap-Activated LED Control

This project uses a KY-038 sound sensor to detect claps and toggle LEDs on and off. It is designed to work with an Arduino board for interactive sound-based control.

🛠 Components Required

🖥 Arduino board

🎙 KY-038 sound sensor (using D0 pin)

💡 3 LEDs

🔌 Resistors (220Ω recommended)

🔗 Jumper wires

🔲 Breadboard

🔌 Wiring Instructions

KY-038 Sound Sensor:

vcc(+)→ Arduino 5V

G → Arduino GND

D0 → Arduino Pin 2

LEDs:

LED1 Anode (+) → Arduino Pin 3

LED2 Anode (+) → Arduino Pin 4

LED3 Anode (+) → Arduino Pin 5

Each LED Cathode (-) → Resistor → GND

⚙️ How It Works

1️⃣ The KY-038 detects a clap and sends a signal to the Arduino.
2️⃣ The Arduino toggles the state of the LEDs.
3️⃣ A short delay prevents multiple triggers from a single clap.

📝 Code Overview

The provided code reads the digital signal from the KY-038 and toggles the LEDs on each clap detection.

🚀 Uploading the Code

1️⃣ Connect your Arduino to the computer.
2️⃣ Open the Arduino IDE and select the correct board and port.
3️⃣ Copy and paste the provided code into the IDE.
4️⃣ Click Upload.

🎮 Usage

👏🏿 Clap once to turn the LEDs ON.

👏🏿 Clap again to turn them OFF.

ℹ️ Notes

✔️ Ensure the KY-038 is adjusted for proper sensitivity.
✔️ If the LEDs are not responding, check wiring and adjust the sensor's sensitivity using the onboard potentiometer.

🚨 Potential Issues & Fixes
🔹 Sensor Not Detecting Claps

Adjust KY-038 sensitivity using the potentiometer.
Ensure wiring is correct (D0 to Pin 2).
Reduce background noise.
🔹 LEDs Not Turning On/Off

Check wiring: anodes to Arduino pins, cathodes to GND via resistors.
Test LEDs separately.
Use Serial Monitor to check if the sensor is detecting signals.
🔹 Multiple Claps Needed

Clap louder or closer to the microphone.
Increase delay(100) to prevent multiple triggers.
🔹 LEDs Stay ON From Start

Set ledState = false; in setup().
Check if the sensor is falsely triggering (Serial.println(digitalRead(SOUND_SENSOR_PIN));).
🔹 False Triggers

Reduce KY-038 sensitivity.
Move away from noisy environments.
🔹 Code Not Uploading

Ensure the correct board & port are selected.
Verify wiring and syntax before uploading.

🕺🏿 Happy coding! 🕺🏿

Youtube Link: https://youtu.be/XoophNz3-IY

Email: d.denvour@outlook.com
