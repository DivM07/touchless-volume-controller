# touchless-volume-controller
A Python application to control system master volume hands-free using OpenCV and MediaPipe

A real-time computer vision utility that allows you to adjust your Windows system's master volume entirely hands-free. By utilizing webcam feed and spatial hand tracking, this application maps the physical distance between your thumb and index finger to your computer's audio levels.

## 🚀 Features

* **Real-Time Hand Tracking:** Utilizes MediaPipe to detect and map 21 distinct 3D hand landmarks via a standard webcam.
* **Dynamic Audio Control:** Interfaces directly with the Windows core audio system via PyCaw to dynamically set the master volume based on gesture distance.
* **On-Screen UI:** Displays a live volume bar, percentage readout, and visual tracking lines directly on the video feed using OpenCV.
* **Distance Mapping:** Employs NumPy interpolation to smoothly convert the pixel distance between fingertips into the accepted system decibel range (0 to 100%).

## 🛠️ Technologies Used

* **Python 3.x**
* **OpenCV (`cv2`):** For webcam video capture, image processing, and rendering the on-screen UI.
* **MediaPipe:** For high-performance, real-time hand landmark detection.
* **PyCaw & Comtypes:** For accessing and manipulating Windows core audio endpoints.
* **NumPy:** For mathematical interpolation and data mapping.
* **Math:** For calculating the hypotenuse distance between finger coordinates.

## ⚙️ Installation & Setup

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/YourUsername/touchless-volume-controller.git](https://github.com/YourUsername/touchless-volume-controller.git)
   cd touchless-volume-controller
