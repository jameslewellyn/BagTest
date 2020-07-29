# BagTest

Ventilators In Peoria (VIP)

Test the VIP fixture

This is written and tested on the Arduino Mega 2560

Serial Port Info:

stty -F /dev/ttyACM0 115200
cu -l /dev/ttyACM0 -s 115200

 ~/arduino-1.8.12/arduino --upload BagTest.ino

Now:

make upload

Collecting Data:

cat /dev/ttyUSB0  | tee DATA/NewMotorData.csv 


