# Vehicle Speed Estimation

This repository contains code for estimating vehicle speeds in a video using object detection and perspective transformation techniques.

## Setup

Before running the code, ensure that you have access to a GPU. You can verify GPU access by running the `nvidia-smi` command. If there are any issues, navigate to `Edit` -> `Notebook settings` -> `Hardware accelerator`, set it to `GPU`, and then click `Save`.

## Installation

To install the required dependencies, run the following command:

!pip install -q supervision ultralytics


## Usage

1. **Download Data**: The code downloads the necessary video data for vehicle speed estimation.

2. **Configuration**: Set the configuration parameters such as video paths, confidence threshold, IOU threshold, model name, and resolution.

3. **Source and Target ROIs**: Define the source and target regions of interest (ROIs) for perspective transformation.

4. **Transform Perspective**: Transform the perspective of the video frames using the defined ROIs.

5. **Process Video**: Process the video frames to estimate vehicle speeds. The code detects vehicles, tracks them, calculates their positions, and annotates the frames with speed labels.

6. **View Result**: The result of the vehicle speed estimation is available below, which provides a visual representation of the annotated vehicle speeds.

![Vehicle Speed Estimation Result](vehicles-result.gif)

## Files

- `vehicle-speed-estimation.ipynb`: Jupyter Notebook containing the code for vehicle speed estimation.
- `vehicles.mp4`: Input video containing footage of vehicles.
- `vehicles-result.mp4`: Output video with annotated vehicle speeds.
- `vehicles-result.gif`: Animated GIF showing the annotated vehicle speeds.

## Dependencies

- `supervision`: Library for computer vision tasks.
- `ultralytics`: Library for object detection using YOLO models.
- `cv2`: OpenCV library for image processing.
- `numpy`: Library for numerical computations.
- `tqdm`: Library for displaying progress bars.

## Credits


For any questions or issues, please contact [Ali](mailto:m.a.charoosaei@gmail.com).