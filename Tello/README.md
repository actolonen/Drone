# Python programs to control a Tello drone

## Installation of djitellpy library

These programs interact with a Tello drone using the `djitellopy` library, which provides a simple interface for controlling the drone and accessing its camera.

The djitellopy library is not available in conda (I use micromamba), and so must be installed using pip. 

1. Install pip in you micromamba environment

% micromamba install pip

2. Install djitello using pip

% pip install djitellopy

## Code to control drone 

### Streaming video
-   [Code](Code/Video/tello_camera.ipynb) to capture a video stream
-   [Code](Code/Video/tello_camera_sensors.ipynb) to capture a sensor data and video stream. Sensor data (battery level) is printed to the video stream window

### Basic flight control
-   [Code](Code/Flight/tello_flight.ipynb) execute basic flight routine (no video)
-   [Code](Code/Flight/tello_camera-flight_threaded.ipynb) to execute a basic flight routine with streaming video showing sensor data (battery level).

### Keyboard control
-   [Code](Code/keyboard_input.ibynb) to capture keyboard inputs from the user
