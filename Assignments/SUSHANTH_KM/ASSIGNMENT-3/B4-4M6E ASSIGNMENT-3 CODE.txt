import RPi.GPIO as PIN
from time import sleep
red=7
yellow=11
green=13
PIN.setup(red,PIN.OUT)
PIN.setup(yellow,PIN.OUT)
PIN.setup(green,PIN.OUT)
while True:
    PIN.output(red,True)
    sleep(4)
    PIN.output(red,False)

    PIN.output(yellow, True)
    sleep(1)
    PIN.output(yellow, False)

    PIN.output(green, True)
    sleep(3)
    PIN.output(green, False)
PIN.cleanup()
