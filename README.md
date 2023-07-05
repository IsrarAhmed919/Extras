# Image Duplicate Detection README
This repository contains a Python script that utilizes the imagehash library to detect duplicate images within a specified directory. The script calculates perceptual hashes for JPEG images and identifies duplicates based on their hash values.

# Features
Scans a directory for JPEG images and detects duplicates.
Utilizes the imagehash library to calculate perceptual hashes.
Applies preprocessing techniques, including removing the alpha channel from RGBA images and applying the Z-transform to the image data.
Outputs a list of duplicate image paths.
#Getting Started
To get started with this script, follow these steps:

## Prerequisites: Make sure you have the following dependencies installed:

Python (version 3.10)

OpenCV (cv2) library

NumPy library

Pillow library

ImageHash library

## Installation: Install the required dependencies using the pip package manager. You can run the following command:

## Usage: Modify the script to specify the directory path where your images are located. Run the script and it will detect and output duplicate image paths.

# Additional Notes
The script assumes that the images are stored in a directory structure where JPEG images are organized in subdirectories within the main directory.

The alpharemover function is used to remove the alpha channel from RGBA images, converting them to RGB format, which is required for some hashing algorithms.

The with_ztransform_preprocess function applies the Z-transform preprocessing to the image data before generating perceptual hashes.

The dhash_z_transformed function is created using the dhash algorithm with the Z-transform preprocessing.

The script utilizes the average_hash algorithm from the imagehash library to calculate perceptual hashes.

The duplicates list contains the paths of all the duplicate images found.

Make sure to adjust the hash_size parameter in the script to control the size of the perceptual hash.

# Acknowledgements
The script utilizes the following libraries:

OpenCV

NumPy

Pillow

ImageHash

# Contributing
Contributions to this project are welcome. Feel free to open issues or submit pull requests for any improvements or bug fixes.
