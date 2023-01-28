# Raspberry pi 4 cooler control
This is a program to automatically turn on and off the raspberry pi 4 cooler depending on the temperature of the processor.
# Installation
Clone the repository:
```
https://github.com/Tima32/raspberry-pi4-cooler-control.git
```
Add to the end of the file ``/etc/rc.local``, before ``exit 0``
```
sudo python /<path-to>/cooler-control.py &
```
# Testing
Testing can be done with this command
```
stress --cpu 8 -t 60
```
After a few seconds, the fan should begin to rotate, after the command is completed, the fan should stop within about 30 seconds.
