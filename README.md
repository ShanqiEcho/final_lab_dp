# Dance Classification and Performance Analysis

## Project Overview
The "Dance Classification and Performance Analysis" project focuses on classifying dance styles and analyzing performance using video data. Leveraging a custom 3D Convolutional Neural Network (Dance3DCNN), the project aims to categorize dance videos into four styles: HipHop, Jazz, Kata, and Taichi. This initiative was inspired by the challenges beginners face in distinguishing dance types and the potential application of tagging short videos based on their dance style. While the model performs well on the training dataset, it faces challenges generalizing to real-world videos like those from TikTok.

---

## Setup Instructions

### Prerequisites
Ensure you have Python 3.8+ installed. Optionally, you can set up a virtual environment for dependency isolation:
```bash
python -m venv dance_env
source dance_env/bin/activate  # For macOS/Linux
```
For Windows:
```bash
dance_env\Scripts\activate
```

### Install Dependencies
Run the following command to install required libraries:
```bash
pip install -r requirements.txt
```
Alternatively, if using Conda, create the environment:
```bash
conda env create -f conda.yml
conda activate dance_env
```

---

## How to Run

### Demo Scripts
To test the project, use the provided demo notebooks:

1. **Photo Classification**
   - Navigate to the `demo/01Photo_Run/` folder.
   - Ensure the `ModelTry.pth` file and test images are present in the folder.
   - Open and run the `Test_Photo_Run.ipynb` notebook to classify photos.

2. **Video Classification**
   - Navigate to the `demo/02Video_Run/` folder.
   - Ensure the `ModelTry.pth` file and test videos are present in the folder.
   - Open and run the `Test_Video_Run.ipynb` notebook to classify videos.


### Expected Output
- The photo classification notebook (`01Photo_Run`) will predict the dance style for each input image and display results.
- The video classification notebook (`02Video_Run`) will process input videos frame by frame, classify each frame, and determine the overall video category based on majority voting.
- Outputs are saved in the respective results directories within each folder.
- For example:
  - Input: A photo of Taichi.
  - Output: `Predicted Style: Taichi`
  - Input: A video of Jazz.
  - Output: `Predicted Style: Jazz`

---

## Pre-trained Model
The pre-trained models can be downloaded from the following link:
- **ModelTry.pth:** [Download from Google Drive](https://drive.google.com/file/d/1r90CLuMJ6Uhwq7tYCTmkuB7nZal2rcXY/view?usp=sharing)

Save this file in the `demo/01Photo_Run/` folder or `demo/02Video_Run/` to ensure the demo scripts can load the model correctly.

---


## Acknowledgments
- Dataset: The data used in this project is sourced from [Kaggle](https://www.kaggle.com/datasets/tapakah68/segmentation-full-body-mads-dataset?resource=download), originally from the [City University of Hong Kong](http://visal.cs.cityu.edu.hk/research/mads-demo/).
- Frameworks and Libraries: PyTorch, NumPy, Matplotlib































