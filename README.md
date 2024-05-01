# Traffing_sign_classification
In this project, we will leverage Convolutional Neural Networks (CNNs) to develop, train, and evaluate a robust traffic sign classification model. TensorFlow and Keras will be our primary tools for implementation. This endeavor tackles a multiclass classification challenge, where the goal is to accurately identify various traffic signs.

# Execute this cell to upload your kaggle API key file (kaggle.json)
    from google.colab import files
    files.upload()

we will start by connecting to kaggle using Api which can be downloaded from your keggle account's setting and uploading it here(upload box)

# install the kaggle API client
    !pip install -q kaggle

install kaggle api using pip

# The Kaggle API Client expects this file to be in ~/. kaggle , so move it there
     !mkdir -p ~/.kaggle 
     !cd kaggle.json  ~/.kaggle/

# This permissions change avoids a warning on Kaggle tools startup .
     ! chmod 600 ~/.kaggle/kaggle.json

Setting up Kaggle using Kaggle API

# Creating directory and changing the current working directory 
     !mkdir traffic_sign_dataset
     %cd traffic_sign_dataset

# Searching for dataset
    !kaggle datasets list -s gtsrb-german-traffic-sign

Searching kaggle for reqruire dataset using search option(-s)with title 'dogbreedidfromcomp'. We can also use different search opetions like searching competitions, notebooks , kernels, datasets, etc.


# Downloading dataset and coming out of directory 

    ! kaggle datasets download meowmeowmeownmew/gtsrb-german-traffic-sign
    %cd ..

    
