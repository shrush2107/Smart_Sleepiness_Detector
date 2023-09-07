# Driver Drowsiness Detection System

## Overview
This Driver Drowsiness Detection System is a Python-based application that uses computer vision techniques to monitor a driver's facial features and detect signs of drowsiness. It also has the gesture recognition module to control the alarm system. It can be used to enhance road safety by alerting drivers when they show signs of fatigue, such as drowsy eyes or yawning.

## Table of Contents
- [Getting Started](#getting-started)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Arguments](#arguments)
- [Other Details](#other-details)

## Getting Started
Follow these instructions to set up and use the Driver Drowsiness Detection System on your system.

## Prerequisites
Before running the application, make sure you have the following prerequisites installed on your system:

- Python (version >= 3.6)
- OpenCV
- Dlib
- imutils
- numpy
- pygame

You can install most of these dependencies using `pip`. For example:

```shell
pip install opencv-python dlib imutils numpy pygame
```

## Installation
1. Clone or download this repository to your local machine.
2. Install the required dependencies as mentioned in the prerequisites section.

## Usage
To use the Driver Drowsiness Detection System, follow these steps:

1. Open a terminal or command prompt.
2. Navigate to the project directory.
3. Run the following command, specifying the path to the landmark predictor and an optional path to an alarm sound file:

```shell
python drowsiness_detection.py -l path/to/landmark_predictor.dat -a path/to/alarm.wav
```

Replace `path/to/landmark_predictor.dat` with the path to the dlib facial landmark predictor model. You can download this model from the [dlib website](http://dlib.net/files/shape_predictor_68_face_landmarks.dat.bz2).

If you have an alarm sound file, provide its path with the `-a` argument.

## Arguments
- `-l` or `--landmark_predictor`: Required. Path to the dlib facial landmark predictor model.
- `-a` or `--alarm`: Optional. Path to an alarm sound file (e.g., a WAV file) to be played when drowsiness is detected.
- `-w` or `--webcam`: Optional. Webcam number (default is 0).

## Other Details
More details can be found at DOI: 10.1109/ICACCS51430.2021.9441756
