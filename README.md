# microcontroller-adventures
ESP32 + micropython + raspberry pi

# Installing picocom
sudo apt-get install picocom

# Connecting with REPL to ESP32
picocom -b 115200 /dev/ttyUSB0

# Controlling a servo
import machine
servo = machine.PWM(machine.Pin(15), freq=60)
servo.duty(40)
servo.duty(115)
servo.duty(77)