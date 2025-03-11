# Mayo Clinic STRIP AI

This repo contains work for a Kaggle competition [Mayo Clinic STRIP AI](https://www.kaggle.com/competitions/mayo-clinic-strip-ai/overview) to classify blood clot origins in ischemic stroke. One of the challenges was image dimensions vary widely. My team's solution was to, instead of resizing (which loses information), images are sliced into fixed-size patches to preserve spatial details with low-information patches filtered out.

Code overview:
1. base_line.ipynb  
   - Loads and preprocesses the data.
   - Defines CNN models (e.g., ResNet, EfficientNet) with custom input and output layers.
   - Contains the training and evaluation loops.

2. data_maker.ipynb  
   - Implements the image slicing function.
   - Splits each image into square patches.
   - Filters patches based on mean intensity to discard empty regions.

3. data_exploration.ipynb  
   - Performs exploratory analysis of the dataset.
   - Visualizes samples of original and sliced images.
   - Checks class distribution and image statistics.

How to run:
- Clone my notebooks to Kaggle.
