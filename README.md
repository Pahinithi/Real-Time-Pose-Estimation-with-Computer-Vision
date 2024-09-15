# Real-Time Pose Estimation with TensorFlow.js and JavaScript

This project showcases a real-time human pose estimation system built with TensorFlow.js and JavaScript. It uses pre-trained machine learning models to detect key points in the human body and predict poses from live camera feeds, all within a web browser. The application combines computer vision techniques with deep learning models to create an interactive experience in real time.

## Table of Contents
- [Introduction](#introduction)
- [Technologies Used](#technologies-used)
- [Features](#features)
- [Setup and Installation](#setup-and-installation)
- [Usage](#usage)
- [Screenshots](#screenshots)
- [Demo](#demo)
- [Project Structure](#project-structure)
- [Future Improvements](#future-improvements)
- [Acknowledgements](#acknowledgements)
- [License](#license)

## Introduction

Pose estimation involves identifying the positions and angles of human body joints (key points) to understand body posture. This application performs real-time pose estimation through the user's webcam, using machine learning models to analyze body positions for a range of applications like fitness tracking, sports analysis, and augmented reality.

By leveraging **TensorFlow.js**, we can run these models entirely in the browser, reducing latency and providing a smooth experience without needing server-side processing.

## Technologies Used

- **TensorFlow.js**: A JavaScript library to run TensorFlow models in the browser.
- **JavaScript**: For frontend interactions and camera handling.
- **HTML/CSS**: For building the user interface.
- **WebRTC API**: To access webcam input.
- **PoseNet / MoveNet Models**: Pretrained pose estimation models from TensorFlow.

## Features

- **Real-time pose estimation** from webcam feed.
- **Detection of 17 key points** on the human body (e.g., nose, eyes, elbows, knees).
- **Visual feedback** with a skeleton overlay showing the detected joints.
- **Fast and lightweight** browser-based application.
- Extensible for various use cases like fitness tracking, gesture recognition, gaming, etc.

## Setup and Installation

### Step 1: Clone the Repository

```bash
git clone https://github.com/Pahinithi/Real-Time-Pose-Estimation-with-Computer-Vision
cd real-time-pose-estimation
```

### Step 2: Install Dependencies

TensorFlow.js can be directly imported via a CDN (Content Delivery Network). You don't need to install TensorFlow.js locally for this project.

Add the following script tags to your `index.html` file:

```html
<script src="https://cdn.jsdelivr.net/npm/@tensorflow/tfjs"></script>
<script src="https://cdn.jsdelivr.net/npm/@tensorflow-models/posenet"></script>
```

### Step 3: Run the Application

You can serve this application using a simple HTTP server. For example, using Python:

```bash
python -m http.server 8000
```

Open a web browser and go to `http://localhost:8000` to launch the pose estimation app.

## Usage

- **Launch the Web Application**: Open the application in a browser.
- **Allow Webcam Access**: The browser will request access to the webcam. Click "Allow."
- **Real-time Detection**: Once the webcam feed is loaded, the application will automatically start detecting body key points in real time.
- **Skeleton Overlay**: Detected key points will be marked, and lines will be drawn to show the connections between them (skeleton).

## Screenshots

<img width="1728" alt="Screenshot 2024-09-15 at 11 05 32" src="https://github.com/user-attachments/assets/d4a17368-5ba9-476a-b22b-9570aec71afd"> <br> <br>

<img width="1728" alt="CV03" src="https://github.com/user-attachments/assets/b9486544-b603-4147-ba6f-149e9faadfce">



## Demo

You can watch a live demo of the **Real-Time Pose Estimation** app [here](https://drive.google.com/file/d/13PpkozMZcUMVChZoLJd9fUdj-bLZtyvA/view?usp=sharing).

The demo shows real-time detection of body joints as the person moves in front of the camera, with the skeleton overlay visualizing key points like shoulders, knees, elbows, and more.

## Project Structure

```bash
real-time-pose-estimation/
├── index.html           # Main web page for real-time pose estimation
├── app.js               # JavaScript logic to handle TensorFlow.js and pose estimation
├── style.css            # Basic styles for the user interface
├── assets/              # Contains images and other assets
├── screenshots/         # Folder with images for README documentation
└── README.md            # Project documentation (this file)
```

## Future Improvements

Here are some potential improvements to enhance the project:

- **Multi-Person Pose Detection**: Extend the application to handle multiple people in the camera feed.
- **Customizable Feedback**: Add different feedback mechanisms like sound alerts or fitness instructions based on detected poses.
- **Performance Optimization**: Further reduce latency by optimizing TensorFlow.js operations and ensuring smooth performance on low-end devices.
- **Gesture-Based Controls**: Enable gesture-based controls to interact with the webpage or other applications.

## Acknowledgements

This project was made possible using the following technologies and models:

- **[TensorFlow.js](https://www.tensorflow.org/js)** for enabling machine learning in the browser.
- **[PoseNet Model](https://www.tensorflow.org/lite/models/pose_estimation/overview)** for human pose detection.
- **[MoveNet Model](https://blog.tensorflow.org/2021/06/introducing-movenet-lightning-fast-and-accurate.html)** for highly efficient and accurate pose estimation.

Special thanks to the TensorFlow community for the open-source libraries and models that power this project.

## License

This project is licensed under the **MIT License**.



## Contact

For any questions or support, please contact:

- **Name**: Pahirathan Nithilan
- **Email**: [nithilan32@gmail.com](mailto:nithilan32@gmail.com)
- **GitHub**: [Pahinithi](https://github.com/Pahinithi)

