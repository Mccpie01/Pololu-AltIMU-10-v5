Pololu AltIMU-10 v5 Gyro, Accelerometer, Compass and Altitude Sensor Module

This repository contains the work of the AltIMU-10 complex sensor module.

Working with sensors such as the accelerometer and Gyro is time-consuming and labor-intensive. And it can be pretty boring at times. I have presented the work I have done with these sensors to the developers as open source in order to be tidy here.

Hope it is useful.
calibration

Sensors such as accelerometers and gyro are very sensitive and noisy modules. Since direct use cannot provide stability, various filters must be applied.

You can find sample studies such as Kalman filter, normalization, weighted standard deviation in the repo.

Calibration example (Kalman Filter); calibration
![calibration](https://github.com/haknkayaa/Pololu-AltIMU-10-v5/blob/main/images/calibration.jpg)

Raw acceleration value read from blue line sensor (single axis)
    Red line Value calculated after Kalman filter (single axis)

visualization

Processing 3.5.4 is used to visualize the data received via real-time serial port on the computer in 3D.

Do not forget to edit the COM port selections while running the processing projects in the "visualization" folder.

![calibration](https://github.com/haknkayaa/Pololu-AltIMU-10-v5/blob/main/images/processing.gif)


Development Environment

    MCU: Teensy 3.6
    Build, Compiler and Debugger: CMake 3.19.3, MinGW64 6.0
    IDE: Jetbrains CLion IDE 2021,
    Framework: PlatformIO Core and CLI
    Visualization/GUI: Processing 3.5.4
    OS: Windows 10 Pro

Communication

Hakan KAYA - mail@hakankaya.kim

English version - Pierre McCarragher - pierremccarragher@hotmail.com


