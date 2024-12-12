# Google's QuickDraw Classification Analysis

The goal of this project is to classify hand-drawn sketches from the [Quick, Draw! Dataset](https://quickdraw.withgoogle.com/data) into one of 345 categories. I explored two machine learning approaches:
1. A Convolutional Neural Network (CNN) for deep learning-based image classification.
2. A Support Vector Machine (SVM) for traditional machine learning classification.

Through this project, I aimed to compare the performance and efficiency of these two approaches on the same dataset.

## The Dataset

The [Quick, Draw! Dataset](https://quickdraw.withgoogle.com/data) is a collection of over 50 million drawings across 345 categories, created by Google as part of their Quick, Draw! game. 
- **When it was created**: The dataset was generated from user drawings during gameplay, which started in November 2016.
- **How long it took**: It took several months to compile the dataset, thanks to the contributions of millions of players around the world.
- **Format**: Each drawing is stored as vector data, which I converted into rasterized 28x28 images to make them compatible with the models in this project.

This dataset provided a rich and diverse source of training data for both the CNN and SVM models with over 2 million images.


## Data Preprocessing

To prepare the data for training, I followed these steps:
- **Downloading**: I used the `quickdraw` library to access and download the dataset.
- **Processing**: The raw data was converted into 28x28 images to standardize the input size.
- **Saving**: Processed images were saved in a structured directory format to make training and validation easier.

### Libraries I Used for Data Preprocessing
- **`quickdraw`**: To download and work with the Quick, Draw! Dataset.
- **`numpy`**: To handle image arrays and process data.
- **`matplotlib`**: To visualize some of the preprocessed images for verification.


## Acknowledgements

- I want to thank **Google** for creating and sharing the Quick, Draw! Dataset, which made this project possible. You can learn more about it [here](https://quickdraw.withgoogle.com/data).
- I also appreciate the tools and libraries I used, including:
  - **TensorFlow/Keras**: For enabling me to build and train the CNN model.
  - **scikit-learn**: For helping me implement and evaluate the SVM model.
- Finally, a big thanks to **OpenAI's ChatGPT** for guiding me in creating the project.

