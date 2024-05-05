# Face Mesh Detection Web Application

This web application uses MediaPipe's Face Mesh solution for real-time facial landmarks detection.

## Features

- Real-time face mesh detection from webcam video feed.
- Visualization of the detected face mesh on a canvas.

## How It Works

The application uses the following technologies:

- **MediaPipe Face Mesh**: This is a lightweight machine learning pipeline for the detection of facial landmarks in real-time.
- **Bulma CSS**: A modern CSS framework based on Flexbox for styling the application.
- **JavaScript**: Used for manipulating the DOM and handling the video feed and canvas drawing.

When the application starts, it begins a video feed from the user's webcam. This feed is then processed frame by frame by the Face Mesh model, which detects facial landmarks and returns their coordinates. These landmarks are then drawn on a canvas overlaying the video feed, effectively creating a "mesh" on the user's face in real-time.

## Setup

To run this application, you simply need to host these HTML and JavaScript files on a server, as the Face Mesh model is loaded directly from a CDN. Note that due to browser security restrictions related to webcam access, this application might not work correctly if run directly from the file system (i.e., by opening the HTML file in a browser).

## Usage

Once the application is running and has access to the webcam, you should see your video feed on the left, and the face mesh overlay on the right. If the face mesh is not appearing, ensure that your face is within the video frame and that there is sufficient lighting.

## Note

This is a basic implementation and may not work perfectly in all conditions. Factors such as lighting, face angle, distance from the camera, etc., can all impact the performance of the face mesh detection.
