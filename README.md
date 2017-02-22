# FRC Vision

Simple script that finds the retroreflective target and exports data values of the target to a Network Table. Deployment for vision was tested with a Raspberry Pi 3 and Nvidia Jetson TK1 running Python version 3.5+ as a coprocessor to the roboRIO.

## Installation

Install numpy

`pip install numpy`

Install OpenCV for Python

`pip install opencv-python`

Ensure that you can export to a NetworkTable

`pip install pynetworktables`


## Deploying with FRC Code

There are WPILib articles on computer vision, you can check out FRC 4914's repos for our implementation. Simply read from the NetworkTable and use those values to your heart's content. If you need help with this, read this article: [Reading array values published by NetworkTables](http://wpilib.screenstepslive.com/s/4485/m/24194/l/479908-reading-array-values-published-by-networktables)

## Known Issues

If you are running a Microsoft Lifecam, we have run into problems in the past with adjusting exposure. I've included a script, `init.sh`, have it run immediately on startup for your Pi or Jetson. This should resolve any issues though I recommend getting an IP camera.
