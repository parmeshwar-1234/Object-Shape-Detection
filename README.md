**Object Shape Detection in Python**

This project is a simple Python script that uses OpenCV to detect the shape of objects in a video stream from a webcam. The script can detect the following shapes:

Triangles
Rectangles
Pentagons
Hexagons
Circles

**Prerequisites**
To run the script, you need to have Python and OpenCV installed on your system. You can install OpenCV using pip:

**Copy code**
pip install opencv-python

**Usage**
Run the script using Python:
**Copy code**
python object_shape_detection.py
Press 'q' to exit the program.

**How it works**
The script captures frames from the webcam and applies the following steps to detect the shape of objects:

Convert the frame to grayscale.
Apply Canny edge detection to the grayscale image.
Find contours in the edge image.
Approximate the contour with a polygon.
Calculate the cosine of all corners of the polygon.
Sort the cosine values in ascending order.
Determine the shape of the contour based on the number of vertices and the minimum and maximum cosine values.
Draw the shape label on the frame.

**The script can detect the following shapes:
**
Triangles: 3 vertices
Rectangles: 4 vertices
Pentagons: 5 vertices
Hexagons: 6 vertices
Circles: Approximately circular shape with a small aspect ratio and a small difference between the calculated area and the actual area of the circle.
Note

The script is a simple example and may not work perfectly for all input images. You can improve the accuracy of the shape detection by adjusting the parameters of the Canny edge detection and contour approximation steps.
