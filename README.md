# Real-time rotten fruit detection using color segmentation 
This is a project for real-time detection of rotten fruit areas and infected leaves aeres based on hsv.
# Problem Statement 
The accurate and timely detection of spoiled fruits and diseased leaves is difficult in agriculture and food. Traditional manual inspection is labor-intensive, subjective, and prone to errors. This project aims to develop an automated system that utilizes the HSV color space for the detection and classification of spoiled fruits and diseased leaves.
# Techniques Employed
- HSV-Based Color Segmentation: Identifies discolored or abnormal patches on leaves that typically indicate disease.
- Morphological Processing: Refines the segmented results using operations like opening and closing to remove noise and enhance detection accuracy.
- Image Analysis: Evaluates the processed images to isolate infected regions and calculates the proportion of the leaf that is damaged.
- Live Webcam Integration: Implements real-time detection using OpenCV to analyze a continuous video stream and highlight diseased areas instantly.
# Workflow of the Program
1. Mode Selection: The user can choose between analyzing a saved image or initiating live detection through a webcam.
2. Static Image Analysis:
* Load and prepare the input leaf image.
* Use HSV color segmentation to spot signs of disease.
* Clean the resulting mask using morphological operations to eliminate small artifacts.
* Display the final image with affected areas highlighted, along with the percentage of the leaf infected.
3. Live Detection via Webcam:
* Stream video from the webcam in real time.
* Continuously detect infected spots using HSV color filtering.
* Mark infected areas with a red overlay.
* Show the live feed with highlighted results.
4. Program Termination: The system can be closed by pressing the 'q' key or manually closing the application window.
# Evaluation Metrics

| **Metric**                 | **Details**                                   |
|---------------------------|-----------------------------------------------|
| Detection Technique       | HSV-based color filtering                     |
| Post-Processing           | Morphological operations (open, close)        |
| Frame Rate (Live Mode)    | ~20–30 frames per second                      |
| Damage Visualization      | Displays percentage of affected leaf area     |

# Result

![Screenshot 2025-05-18 at 11 05 09 PM](https://github.com/user-attachments/assets/4b98c697-cf4a-4453-9935-586000338dad)


