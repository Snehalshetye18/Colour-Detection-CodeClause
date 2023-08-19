# Colour-Detection-CodeClause

This repository contains a Python application for color detection in images. The application processes images and identifies prominent colors present within them. This README provides an overview of the project, its structure, and instructions for usage.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Examples](#examples)

## Introduction

Color detection is a common computer vision task that involves identifying the primary colors in an image. This repository provides a simple Python application that uses image processing techniques to extract the dominant colors from input images.

## Features

- **Color Detection:** The application identifies the dominant colors in an image.
- **RGB and HEX Values:** The detected colors are presented in both RGB and HEX color code formats.
- **Image Preview:** The application displays the original image and highlights the detected colors.
- **Command-Line Interface:** Run the application from the command line with customizable parameters.

## Requirements

- Python 3.5+
- OpenCV library (`pip install opencv-python`)
- NumPy library (`pip install numpy`)

## Installation

1. Clone this repository to your local machine using:
   ```
   git clone https://github.com/yourusername/color-detection.git
   ```
   
2. Navigate to the repository directory:
   ```
   cd color-detection
   ```

3. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```

## Usage

Run the color detection application with the following command:
```
python color_detection.py --image path/to/your/image.jpg
```

Replace `path/to/your/image.jpg` with the path to the image you want to process.

Optional arguments:
- `--num_colors`: Number of dominant colors to identify (default is 5).
- `--show_preview`: Display the original image and color highlights (add this flag to show the preview).
- `--output_file`: Save the color information to a CSV file.

## Examples

1. Detect the top 5 colors in an image and display the preview:
   ```
   python color_detection.py --image images/sample.jpg --show_preview
   ```

2. Identify the top 10 colors in an image and save the results to a CSV file:
   ```
   python color_detection.py --image images/another_sample.png --num_colors 10 --output_file colors.csv
   ```
