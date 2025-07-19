# Python programs to control a Tello drone

## References

-   Jacob Pitsenberger's [Github](https://github.com/Jacob-Pitsenberger?tab=repositories) and [Youtube channel](https://www.youtube.com/playlist?list=PLAu6u02VrrtzcivPSOqV5EHZWqmUyEX2o)
-    Raj Paramananda's [Youtube video](https://www.youtube.com/watch?v=FirMJh0_Lw8&t=286s) on using pygame for keyboard input

## Installation of djitellpy library

These programs interact with a Tello drone using the `djitellopy` library, which provides a simple interface for controlling the drone and accessing its camera.

The djitellopy library is not available in conda (I use micromamba), and so must be installed using pip.

1.  Install pip in you micromamba environment

\% micromamba install pip

2.  Install djitello using pip

\% pip install djitellopy

## Code to control drone

### Streaming video

-   [Code](Code/Video/tello_camera.ipynb) to capture a video stream
-   [Code](Code/Video/tello_camera_sensors.ipynb) to capture a sensor data and video stream. Sensor data (battery level) is printed to the video stream window

### Basic flight control

-   [Code](Code/Flight/tello_flight.ipynb) execute basic flight routine (no video)
-   [Code](Code/Flight/tello_camera-flight_threaded.ipynb) to execute a basic flight routine with streaming video showing sensor data (battery level).

### Keyboard control

-   [Code](Code/Keyboard/keyboard_input.ibynb) to capture keyboard inputs from the user and print to STDOUT
-   [Code](Code/Keyboard/keyboard_flight.ipynb) to control drone flight using the keyboard
-   [Code](Code/Keyboard/keyboard_flight-video.ipynb) to control drone flight using the keyboard