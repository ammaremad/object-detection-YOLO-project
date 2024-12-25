# YOLOv5 Object Detection Application

## Overview

This project is a Python application that implements real-time object detection using the YOLOv5 (You Only Look Once version 5) model. It allows users to process video streams from files or webcams, displaying detected objects with bounding boxes and labels. The application features a simple graphical user interface (GUI) built with Tkinter, enabling users to set a confidence threshold for detections and save processed videos.

## Features

- Real-time object detection using YOLOv5.
- Supports video input from files or webcam.
- Adjustable confidence threshold for detection results.
- Option to save processed video output.
- User-friendly GUI built with Tkinter.
- Displays frames per second (FPS) for performance monitoring.

## Requirements

- Python 3.6 or higher
- Libraries:
  - OpenCV
  - PyTorch
  - Tkinter

You can install the required libraries using pip:

```bash
pip install opencv-python torch torchvision torchaudio
```

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/ammaremad/yolov5-object-detection.git
   cd yolov5-object-detection
   ```

2. Install the required libraries as mentioned above.

3. Ensure you have the YOLOv5 model weights downloaded. The model will be automatically downloaded when you run the application for the first time.

## Usage

1. Run the application:

   ```bash
   python app.py
   ```

2. The GUI will open, allowing you to:
   - Set the confidence threshold (between 0 and 1).
   - Load a video file by clicking the "Load Video" button.
   - Use the webcam by clicking the "Use Camera" button.

3. Press 'q' to exit the video stream.

4. You will be prompted to enter a path to save the processed video. If no path is provided, the default name `output_video.avi` will be used.

## Code Structure

- `app.py`: Main application file containing the implementation of the object detection and GUI.
- `requirements.txt`: List of required Python packages.

## Notes

- The application uses the YOLOv5 small model (`yolov5s`) for object detection.
- Ensure your system has a compatible GPU for optimal performance. The application will automatically use the GPU if available.
- You may encounter warnings related to deprecated functions in the PyTorch library. These can be ignored for now, but consider updating the code to use the latest functions in future versions.

## Acknowledgments

- YOLOv5 by Ultralytics for the object detection model.
- OpenCV for video processing capabilities.
- Tkinter for the graphical user interface.

Feel free to contribute to this project by submitting issues or pull requests!
