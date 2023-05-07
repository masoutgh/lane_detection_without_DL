# lane_detection_without_DL
Real-time Lane Detection Using Basic Computer Vision Techniques
his repository contains a Python implementation of real-time lane detection using basic computer vision techniques. The code uses OpenCV library for image processing.

Requirements
Python 3.x
OpenCV-Python library
Numpy library
Usage
To run the code, clone this repository to your local machine and navigate to the project directory in a terminal window.

bash
git clone https://github.com/<username>/lane-detection.git
cd lane-detection
Then, run the lane_detection.py script using the following command:

bash
python lane_detection.py
Algorithm Overview
The lane detection algorithm used in this code follows these basic steps:

Load the input video stream.
Convert the video frames to grayscale.
Apply Gaussian blur to the grayscale frames to smooth out any noise and make the edges more pronounced.
Use Canny edge detection algorithm to detect edges in the blurred grayscale frames.
Define a region of interest (ROI) for the video frames where the lane markings are expected to appear. Discard edges outside of this area and focus only on the relevant parts of the frames.
Detect lines using Hough transform in the ROI. The Hough transform converts detected edge points into lines in the parameter space.
Draw the detected lines back onto the original color frames to visualize the results in real-time.
Results
The output of the lane detection code will be displayed in a new window, showing the real-time lane detection results. The detected lanes are highlighted with red color lines.

Contributing
If you have suggestions or find bugs, please file an issue on the GitHub repository. Pull requests are welcome.

License
This code is released under the MIT License.

Acknowledgements
The lane detection algorithm used in this code is inspired by the following papers:

Canny, J. (1986). A computational approach to edge detection. IEEE Transactions on Pattern Analysis and Machine Intelligence, 8(6), 679-698.
Hough, P. V. C. (1962). Method and means for recognizing complex patterns. US Patent 3,069,654.
