# Text Detection and OCR using EAST and pytesseract

This project demonstrates the use of the EAST (Efficient and Accurate Scene Text) text detection model and pytesseract for optical character recognition (OCR) to detect and extract text from images.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Code Overview](#code-overview)
- [Contributing](#contributing)
- [License](#license)

## Introduction

This project uses the EAST text detection model and pytesseract to detect and extract text from images. The code snippet provided demonstrates the implementation of the text detection and OCR functionality.

## Features

- Text detection using the EAST model.
- Optical character recognition (OCR) using pytesseract.
- Drawing bounding boxes around detected text.
- Extracting text from the detected bounding boxes.

## Getting Started

1. Clone the repository: `git clone https://github.com/username/projectname.git`
2. Install the required dependencies:
   - OpenCV (`cv2`)
   - NumPy (`np`)
   - Matplotlib (`plt`)
   - pytesseract (`pytesseract`)
   - Roboflow (`Roboflow`)
3. Download the pre-trained EAST text detection model from [https://github.com/argman/EAST](https://github.com/argman/EAST) and save it as `frozen_east_text_detection.pb` in your project directory.

## Usage

1. Replace `image_paths[0]` with the path to the image you want to process.
2. Run the code.
3. The code will display the image with bounding boxes around the detected text and print the detected texts.

## Code Overview

The provided code snippet demonstrates the implementation of the text detection and OCR functionality using the EAST model and pytesseract. The code includes the following functions:

- `preprocess_image`: Preprocesses an image by resizing it and normalizing the pixel values.
- `decode_predictions`: Decodes the predictions made by the EAST model.
- `non_max_suppression`: Performs non-maximum suppression to remove overlapping bounding boxes.
- `detect_text`: Detects text in an image using the EAST model.
- `draw_boxes_and_extract_text`: Draws bounding boxes around detected text and extracts the text using pytesseract.

## Contributing

Contributions are welcome! If you find any bugs or have any suggestions for improvements, please feel free to open an issue or submit a pull request.

## License

This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).
