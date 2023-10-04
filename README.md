# aanishakumari-cc-project-
# Import libraries
import RPi.GPIO as GPIO
import time
# Set up GPIO pin for smoke sensor
SMOKE_SENSOR_PIN = 18
GPIO.setmode(GPIO.BCM)
GPIO.setup(SMOKE_SENSOR_PIN, GPIO.IN)
# Wait for smoke sensor to detect smoke
while not GPIO.input(SMOKE_SENSOR_PIN):
 time.sleep(0.1)
# Smoke has been detected
print("Smoke detected!")
This code uses the Raspberry Pi's GPIO pins to interface with a smoke sensor. It waits for the sensor to detect 
smoke, and then prints a message indicating that smoke has been detected.
Fire Prevention:
# Import libraries
import RPi.GPIO as GPIO
import time
# Set up GPIO pin for fire prevention system
FIRE_PREVENTION_PIN = 17
GPIO.setmode(GPIO.BCM)
GPIO.setup(FIRE_PREVENTION_PIN, GPIO.OUT)
# Turn on fire prevention system
GPIO.output(FIRE_PREVENTION_PIN, GPIO.HIGH)
time.sleep(60) # Keep system on for 60 seconds
# Turn off fire prevention system
GPIO.output(FIRE_PREVENTION_PIN, GPIO.LOW)

