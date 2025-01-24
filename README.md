# Suspicious Crowd Activity Detection and Localization

This project leverages Computer Vision and Convolutional Neural Networks (CNN) to detect suspicious activities in real-time from CCTV surveillance footage. It aims to improve security by providing an automated approach for identifying anomalies in crowded spaces like malls, airports, and railway stations.

#Features
	•	Real-time detection and localization of suspicious activities.
	•	Categorization of activities into:
	1.	Suspicious Activity
	2.	Criminal Activity
	3.	General (Safe) Activity
	•	Integration with YOLO (You Only Look Once) for object detection.
	•	Sends automated alerts upon detecting anomalies.
	•	Uses CNN and LSTM for accurate temporal and spatial analysis of video frames.

#System Overview

Methodology:
	1.	Input Video Stream: Live or recorded surveillance footage.
	2.	Preprocessing: Noise reduction, normalization, and frame extraction.
	3.	Object Detection: Detects humans and activities using a YOLOv4 model.
	4.	Classification: Categorizes activities using a hybrid CNN-LSTM model.
	5.	Alert System: Generates alerts upon detecting suspicious activities.

Tools and Technologies:
	•	Python
	•	YOLOv4 (object detection)
	•	CNN (for feature extraction)
	•	LSTM (for temporal pattern recognition)
	•	Libraries: OpenCV, TensorFlow, Keras

#Project Architecture
	1.	Video Input: Captures video from CCTV cameras.
	2.	Preprocessing: Converts video into frames, resizes them, and normalizes.
	3.	Model Training:
	•	Trained on datasets from Kaggle, YouTube, and public surveillance videos.
	•	Focused on actions like fighting, theft, or unusual gatherings.
	4.	Detection & Classification:
	•	Uses ResNet50 and YOLO for identifying suspicious behaviors.
	•	Combines spatial (images) and temporal (sequence of images) analysis.
	5.	Output:
	•	Generates visual alerts on the video feed.
	•	Sends notifications to designated authorities.

#Dataset

Sources:
	•	Kaggle Dataset: Criminal and suspicious activity data.
	•	Custom Dataset: Created using YouTube videos and public footage.

Preprocessing:
	•	Frames resized to 64x64 pixels.
	•	Normalized pixel values for better processing.

Dataset Categories:
	1.	Fighting
	2.	Walking
	3.	Running

#Installation

Prerequisites:
	•	Python 3.8+
	•	Virtual environment (optional but recommended)

Steps:
	1.	Clone the repository:

git clone https://github.com/NaiduBM/HUMAN-SUSPICIOUS-ACTIVITY-FLASK.git


	2.	Navigate to the project directory:

cd suspicious-activity-detection


	3.	Install dependencies:

pip install -r requirements.txt


	4.	Download pretrained YOLOv4 weights and place them in the models/ directory.

Usage

Running the Application:
	1.	Start the surveillance system:

python main.py


	2.	Select the video feed type (Live or Recorded).
	3.	Monitor the console/logs for detection alerts.

Output:
	•	Detected anomalies are highlighted in the video feed.
	•	Alerts are sent to the administrator via email/SMS.

Results
	•	Accuracy:
	•	Kaggle Dataset: 95.5% with ResNet50.
	•	Real-time Video: 99.01% with ResNet50.
	•	Performance: Real-time processing with minimal computational overhead.

Future Work
	•	Enhanced storage services for archived footage.
	•	Improved real-time processing for high-definition video.
	•	Integration with advanced alert mechanisms (e.g., mobile push notifications).

#License

This project is licensed under the MIT License. See the LICENSE file for details.

Let me know if you’d like further customization!
