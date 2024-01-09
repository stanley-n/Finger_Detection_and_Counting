# Finger Detection and Counting
This project is aimed at detecting and counting fingers using computer vision techniques. It utilizes OpenCV and NumPy libraries in Python to process live camera feeds and perform finger counting based on hand gestures. 


https://github.com/stanley-n/Finger_Detection_and_Counting/assets/81343463/985f422e-263f-42b7-b170-d4901b176edc


## Overview
The project involves several key steps:

•	Calculating the average background value to identify hand regions effectively.

•	Segmenting the hand region in the frame using background subtraction techniques.

•	Utilizing Convex Hulls to calculate fingers and count them based on certain criteria.

## Installation
To use this project, ensure you have the following dependencies installed:

  - python=3.6
  - opencv
  - scikit-learn
  - matplotlib
  - numpy
  - scipy
  - keras
  - tensorflow=1.14

Clone the repository and run the main script to start the finger detection and counting application.

## Usage
1.	Ensure your camera is on.
2.	Run the `main.ipynb` script.
3.	The application will initialize and begin calculating the background average for the first 60 frames. Wait for at least 5 seconds before inserting hand into red bounding box displayed on screen.
4.	Once the hand is inserted into red bounding box, it will segment the hand region and display the count of detected fingers in real-time.

## Code Structure
The code is organized into the following major sections:
•	Imports: Necessary libraries and modules are imported.

•	Global Variables: Variables used throughout the program are defined.

•	Functions: Definitions for key functions like `calc_accum_avg`, `segment`, and `count_fingers`.

•	Run Program: Main execution loop that captures the camera feed and performs finger counting.

## Customization
Feel free to adjust the `threshold` value for better hand detection based on your background. You can also modify the radius within the `count_fingers` function to optimize finger counting based on your hand size.

## Acknowledgments
This project was inspired by a course on Udemy taught by Jose Portilla.

## License
This project is not licensed.
