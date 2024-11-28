# Evaluation Framework for Synthetic Human Action Recognition-1b

## Introduction

In the field of synthetic human action recognition, it is crucial to evaluate the quality and realism of generated videos. One effective way to achieve this is by calculating the Fréchet Inception Distance (FID) and Fréchet Video Distance (FVD) scores between real and synthetic videos. These metrics help in quantifying the similarity between the distributions of real and synthetic data, providing a reliable measure of the synthetic video's quality.

## Team Members

Nivruthi Narayana – SE21UARI102
Nikitha Punati – SE21UARI100
Niketana Bumireddy – SE21UARI098
Mounika Reddy – SE21UARI084
## Dataset for Real Videos

The dataset for real videos can be found at [sims4action](https://github.com/aroitberg/sims4action?tab=readme-ov-file).

## FID/FVD Metrics

This repository provides a comprehensive toolkit for computing Fréchet Inception Distance (FID) and Fréchet Video Distance (FVD) metrics. These metrics are widely used for evaluating the quality of generative models in image and video generation.

## Installation

1. **Clone the repository:**
    ```sh
    git clone https://github.com/pranav190232/fid-metrics.git
    ```

2. **Create a new virtual environment:**
    ```sh
    python -m venv env
    ```

3. **Activate the virtual environment:**
    - On Windows:
      ```sh
      .\env\Scripts\activate
      ```
    - On macOS/Linux:
      ```sh
      source env/bin/activate
      ```

4. **Install the required packages:**
    ```sh
    pip install hydra-core opencv-python pillow rich scipy torch torchvision
    ```

5. **Trim the synthetic video duration for high throughput and less processing time (optional).**

6. **Update the `config.yaml` file**:
   In the `config.yaml` file, specify the path to your [i3d_pretrained_400.pt](http://_vscodecontentref_/3) file:
   ```yaml
   model:
      path: path\to\your\i3d_pretrained_400.pt
   ```

7. **Go to the `app.py` code and place your respective GitHub folder paths as needed.**

8. **Run the application:**
    ```sh
    python app.py
    ```
9. **then use ur results to plot the graph using graph.py**

## Usage

After setting up the environment and installing the necessary packages, you can use the provided scripts to compute FID and FVD scores for your generative models. Simply run the application and follow the on-screen instructions to drag and drop your video files.

For more detailed information, please refer to the documentation or the help command within the application.
#
