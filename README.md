# Object Detection and Tracking with Supervision and Roboflow

This repository contains a Google Colab notebook demonstrating object detection and tracking using the `supervision`, `inference`, and `roboflow` libraries. The notebook is specifically designed to detect and track tennis balls in images and videos using a pre-trained model from Roboflow.

## Project Overview

The project utilizes a combination of powerful computer vision tools to:

1.  **Perform object detection:** Identify the location of specific objects (tennis balls) within an image or video frame.
2.  **Track objects:** Follow the movement of detected objects across consecutive frames in a video.
3.  **Annotate results:** Visualize the detection and tracking results by drawing bounding boxes and labels on the original media.

The workflow includes installing necessary libraries, setting up API access to Roboflow, performing inference on both still images and video sequences, and saving the processed video.

## Setup

To run this notebook, you will need:

1.  A Google account to access Google Colab.
2.  A Roboflow account and an API key. You can obtain one by signing up on the [Roboflow website](https://roboflow.com/).
3.  Access to the specified tennis ball detection model on Roboflow (ID: `tennistracker-95wb6/1`).

### Steps to Run the Notebook

1.  Open the `.ipynb` file in Google Colab.
2.  Ensure you have connected your Google Drive to Colab if you are using files stored there.
3.  Replace the placeholder `""` in the "Set Roboflow API Key" section with your actual Roboflow API key.
4.  Update the image and video file paths in the "Image Inference and Annotation" and "Video Inference and Tracking" sections to point to your desired media files.
5.  Run each code cell sequentially.

## Code Description

The notebook is structured into several key blocks:

-   **Install Libraries:** Installs `supervision`, `inference`, and `roboflow`.
-   **Import Libraries:** Imports necessary modules for image processing, object detection, and tracking.
-   **Set Roboflow API Key:** Configures the environment variable for Roboflow authentication.
-   **Image Inference and Annotation:** Demonstrates object detection on a single image and visualizes the results.
-   **Video Inference and Tracking:** Performs object detection and tracking on a video, saving the annotated video to a file named `out.mp4`.

## Dependencies

The primary dependencies used in this notebook are:

-   `supervision`
-   `inference`
-   `roboflow`
-   `opencv-python` (imported as `cv2`)

These libraries are installed automatically when you run the first code cell.

## Usage

After running the notebook, you will:

-   See an annotated image displayed showing detected tennis balls.
-   Generate a new video file named `out.mp4` in your Colab environment, containing the original video with detected and tracked tennis balls annotated with bounding boxes.
