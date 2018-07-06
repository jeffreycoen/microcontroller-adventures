# microcontroller-adventures
ESP32 + micropython + raspberry pi


# Connecting with REPL to ESP32
picocom -b 115200 /dev/ttyUSB0

# Controlling a servo
servo = machine.PWM(machine.Pin(15), freq=60)
servo.duty(40)
servo.duty(115)
servo.duty(77)