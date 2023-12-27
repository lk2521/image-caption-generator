# Image Caption Generator using Deep Learning
This project utilizes Deep Learning techniques to generate captions for images using the [Flicker_8k Dataset](https://github.com/jbrownlee/Datasets/releases/download/Flickr8k/Flickr8k_Dataset.zip) and [Flickr_8k_text](https://github.com/jbrownlee/Datasets/releases/download/Flickr8k/Flickr8k_text.zip).

## Overview
The goal of this project is to train a model to generate descriptive captions for images by leveraging deep learning technologies. It uses the powerful Xception model for feature extraction and an LSTM-based neural network for generating text captions.

## Getting Started
To set up the project, follow these steps:

### Installation
* Ensure you have the necessary packages installed:
* `pip install tensorflow keras pillow numpy tqdm`

### Dataset Preparation
1. Download the [Flicker_8k Dataset](https://github.com/jbrownlee/Datasets/releases/download/Flickr8k/Flickr8k_Dataset.zip) and [Flickr_8k_text](https://github.com/jbrownlee/Datasets/releases/download/Flickr8k/Flickr8k_text.zip).
2. Organize the dataset into the specified directories:
  * `data_dir/image` for image data.
  * `data_dir/text` for text data.

### Training the Model
1. Load the dataset and perform data cleaning.
2. Extract feature vectors from images using the Xception model.
3. Tokenize the vocabulary and create data generators.
4. Define and train the CNN-LSTM model.

### Testing the Model
1. Use the trained model to generate captions for images.

## Project Structure
* `data_dir/`: Contains image and text datasets.
* `models/`: Stores trained model checkpoints.
* `tokenizer.p`: Pickled tokenizer file.

## License
* This project is licensed under the MIT License.

## Improvement
* **Larger Dataset Integration**: Incorporating a more extensive dataset of approximately 100,000 images and their respective captions could profoundly enhance the model's accuracy and diversity in generating captions.

* **Extended Training Epochs**: Extending the number of epochs beyond the current 10 iterations during the model training phase would likely yield improved performance, refining the model's ability to generate more accurate and nuanced captions.
