# Optical Mark Recognition (OMR) System

## Overview
This project is an **Optical Mark Recognition (OMR) System** built using **OpenCV** and **NumPy**. It processes scanned or photographed multiple-choice answer sheets to detect marked responses automatically.

## Features
- **Preprocess Images**: Convert to grayscale, apply blurring, and thresholding.
- **Detect Bubbles/Marks**: Identify filled options using contour detection.
- **Analyze Responses**: Compare detected answers with the correct ones.
- **Generate Results**: Output student scores and marked sheets.

## Installation
Make sure you have Python installed, then install the required libraries:

```bash
pip install opencv-python numpy
```

## Usage
1. **Prepare your OMR Sheet:** Ensure a clear image of the filled answer sheet.
2. **Run the Script:** Execute the Python file with the scanned image.
   
   ```bash
   python omr_system.py --image path/to/your/image.jpg
   ```
3. **View Results:** The script will display the detected marks and provide score analysis.

## File Structure
```
OMR-System/
│── omr_system.py        # Main script for OMR processing
│── test_images/         # Sample OMR sheets for testing
│── results/             # Processed answer sheets and scores
│── README.md            # Project documentation
```

## Example Output
The system will highlight marked answers and output the results as follows:
```
Student Score: 8/10
Detected Answers: ['A', 'B', 'C', 'D', 'B', 'A', 'C', 'D', 'A', 'B']
```

## Future Enhancements
- Implement machine learning for improved accuracy.
- Support different OMR sheet templates.
- Web interface for online OMR checking.

## Contributing
Feel free to fork this repository and contribute improvements!

## License
This project is licensed under the MIT License.

