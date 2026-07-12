# Real-Time Color Detection Using Webcam

A real-time color detection project built with Python, OpenCV, pandas, and pyttsx3. It captures live webcam frames, detects the color at the selected point, matches it with a dataset, and gives voice feedback.

## Features

* Real-time webcam color detection
* Dataset-based color matching
* Voice output using text-to-speech
* Capture-based color recognition
* Simple and lightweight design
* Runs from a Jupyter Notebook

## Tech Stack

* Python
* OpenCV
* pandas
* pyttsx3
* NumPy
* Jupyter Notebook

## Project Structure

```bash
Color_Detection_Model_Using_Deep_Learning/
│
├── Main.ipynb
├── colors_cleaned_final.csv
└── README.md
```

## Dataset Format

The dataset should contain RGB values and the corresponding color label.

Expected columns:

* `red`
* `green`
* `blue`
* `label`

Example:

| red | green | blue | label |
| --- | ----- | ---- | ----- |
| 255 | 255   | 255  | White |
| 0   | 0     | 0    | Black |

## How It Works

1. The webcam captures a live frame.
2. The center pixel color is read in RGB format.
3. That RGB value is compared with the dataset.
4. The closest matching color label is detected.
5. The detected color is shown on screen and spoken aloud.

## Installation

Clone the repository:

```bash
git clone https://github.com/Mayank-Dandane/Color_Detection_Model_Using_Deep_Learning.git
cd Color_Detection_Model_Using_Deep_Learning
```

Install the required packages:

```bash
pip install opencv-python pandas pyttsx3 numpy
```

## How to Run

Open `Main.ipynb` in Jupyter Notebook and run all cells.

Or, if you convert the notebook into a Python script, run:

```bash
python main.py
```

## Controls

* Press `c` to capture and recognize the current color
* Press `q` to stop detection and exit

## Output

The detected color is displayed on the video frame and announced through voice feedback.

## Limitations

* Detection accuracy may change with lighting conditions
* Very similar shades can be mapped to the same label
* Webcam quality affects the output
* The current version is more color matching based than deep learning based

## Future Improvements

* Add a proper GUI with buttons
* Improve detection under different lighting
* Support more color categories
* Add smoother frame processing
* Convert the notebook into a full Python application


## Author

**Mayank Dandane**
