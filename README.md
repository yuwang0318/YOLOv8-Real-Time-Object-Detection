# YOLOv8-Real-Time-Object-Detection
This project demonstrates web based real-time object detection using YOLOv8 and OpenCV, served through a Flask web application. The application captures video from a webcam, processes it with a YOLOv8 model, and streams the video with detected objects highlighted.

## Features

- Real-time object detection using YOLOv8
- Web-based interface for viewing the video stream
- Simple and clean UI

## Project Structure

```
YOLOv8-Real-Time-Object-Detection/
│
├── app.py                   # Main application file
├── requirements.txt         # Python dependencies
├── templates/
│   └── index.html           # HTML template for the web interface
└── yolo-Weights/
    └── yolov8n.pt           # YOLOv8 model weights
```

## Requirements

- Python 3.x
- Flask
- OpenCV
- Ultralytics YOLO

## Installation

1. **Clone the Repository**

   ```bash
   git clone https://github.com/yuwang0318/YOLOv8-Real-Time-Object-Detection.git
   cd your-repo-name
   ```

2. **Create a Virtual Environment**

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. **Install Dependencies**

   ```bash
   pip install -r requirements.txt
   ```

   Ensure your `requirements.txt` includes:
   ```
   Flask==2.3.2
   opencv-python==4.8.0.74
   ultralytics==8.0.0
   ```

4. **Download YOLOv8 Weights**

   Download the YOLOv8 weights file and place it in the `yolo-Weights` directory.

## Usage

1. **Run the Application**

   ```bash
   python app.py
   ```

2. **Access the Web Interface**

   Open your web browser and go to `http://127.0.0.1:5000/` to view the real-time object detection stream.

3. **Stop the Stream**

   To stop the video stream, access `http://127.0.0.1:5000/stop`.

## Customization

- **Camera Input**: Change the camera index in `app.py` to switch between different camera inputs.
- **UI Design**: Modify `index.html` to customize the look and feel of the web interface.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [Ultralytics YOLO] for the YOLOv8 model
- [OpenCV](https://opencv.org/) for computer vision capabilities
- Reference https://dipankarmedh1.medium.com/real-time-object-detection-with-yolo-and-webcam-enhancing-your-computer-vision-skills-861b97c78993
