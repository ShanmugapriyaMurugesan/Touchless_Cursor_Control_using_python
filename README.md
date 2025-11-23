# HandGuesture using python 
This project implements a real-time hand gesture recognition system in Python using MediaPipe and OpenCV to control mouse actions. It allows users to move the cursor, perform clicks, and drag-and-drop using hand gestures detected from a webcam. Note that volume and brightness control features are not supported in this version.
# Features
   * Cursor movement controlled by hand gestures
   * Left click, right click, double click
   * Drag-and-drop functionality
   * Supports recognition of major (dominant) and minor (non-dominant) hands for different gesture mappings
   * Real-time visual feedback of hand landmarks shown in an OpenCV window

# Dependencies
      opencv-python — for webcam capture and display
      mediapipe — for hand landmark detection and gesture recognition
      pyautogui — to simulate mouse movements and clicks
      comtypes, google.protobuf — auxiliary libraries

# Install dependencies using:
    pip install opencv-python mediapipe pyautogui comtypes protobuf
# How It Works
  *Captures video continuously from your webcam.
  *Uses MediaPipe Hands to detect and track hand landmarks.
  *Converts detected finger positions into gesture encodings.
  *Maps recognized gestures to mouse controls such as moving the cursor, clicking, and dragging.
  *Differentiates between major and minor hands for more robust gesture recognition.

# Usage
    Run the script by executing:
    gc1 = GestureController()
    gc1.start()
A window will appear showing your webcam feed with hand landmarks drawn. Use your hand gestures in front of the camera to move the mouse 
cursor and perform drag-and-drop actions.
# Limitations
  * This version does NOT support system volume or brightness control.
  * Only cursor movement and mouse button interactions are implemented.
  * Volume and brightness functionalities seen in code are placeholders and currently inactive.
# Credits
  * Built using MediaPipe Hands for hand landmark detection.
  * Inspired by computer vision and gesture control research projects.


