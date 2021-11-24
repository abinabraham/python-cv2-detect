# python-cv2-detect

Face and Eyes Recognition with Python

OpenCV is the most popular library for computer vision. Originally written in C/C++, it now provides bindings for Python.

Installing OpenCV
here you will get the instructions https://opencv.org/releases/

Important Parts:-
# Read the image
image = cv2.imread(imagePath)
gray = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)

Here we read the image and convert it to grayscale. Many operations in OpenCV are done in grayscale.

# Detect faces in the image
faces = faceCascade.detectMultiScale(
    gray,
    scaleFactor=1.1,
    minNeighbors=5,
    minSize=(30, 30),
    flags = cv2.cv.CV_HAAR_SCALE_IMAGE
)
For Webcam

OpenCV grabs each frame from the webcam, and you can then detect faces by processing each frame.

Sample Testing

'''python3 face_detect.py doll.jpg'''
