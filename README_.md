# Melanoma detection assignment 
>The goal of this project is to develop a CNN-based model for the accurate detection of melanoma, a deadly skin cancer responsible for 75% of skin cancer-related deaths. Early detection is critical, and a solution capable of evaluating images to alert dermatologists about the presence of melanoma has the potential to significantly reduce manual diagnostic effort.

## Table of Contents
* [Problem Statement](#problem-statement)
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)

<!-- You can include any other section that is pertinent to your problem -->

## Problem Statement
The objective of this project is to develop a CNN-based model for the accurate detection of melanoma, a deadly form of skin cancer responsible for 75% of skin cancer-related deaths. Early detection is crucial, and an automated solution that evaluates images and alerts dermatologists about potential melanoma can significantly reduce the manual effort required in diagnosis.

## General Information

> The dataset comprises 2,357 images of both malignant and benign skin conditions, sourced from the International Skin Imaging Collaboration (ISIC). The images are classified according to ISIC guidelines, with subsets balanced in number, except for melanomas and moles, where the number of images is slightly skewed towards melanomas.

- The data set contains the following diseases:
    - Actinic keratosis
    - Basal cell carcinoma
    - Dermatofibroma
    - Melanoma
    - Nevus
    - Pigmented benign keratosis
    - Seborrheic keratosis
    - Squamous cell carcinoma
    - Vascular lesion
> Using CNN to classify 9 different skin cancer diseases. This will certainly reduce manual effort and prioritize treatment as timely detection of these diseases is the key.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- Augmentation strategy applied to overcome the class imbalance and reducing overfitting, underfitting issues
- Images are normalized between 0-1 and resized to 180*180
- seborrheic keratosis shows minimum number of samples and pigmented benign keratosis have higher number of samples
- Dropout layers are included to reduce overfitting
- The Final model gives below accuracies after 30 epochs
    - Training accuracy - 78.93%% 
    - Validation accuracy -  76.76%  

##Conclusion:
The results of this melanoma detection model demonstrate solid performance in both training and validation phases. After applying class rebalancing techniques, the model achieved the following key metrics:

- Training Accuracy: 78.93%
- Validation Accuracy: 76.76%
- Training Loss: 0.7344
- Validation Loss: 0.6942
### Model Performance:
The close proximity between training accuracy (78.93%) and validation accuracy (76.76%) is a positive sign of the model's ability to generalize well to new, unseen data. A small gap between the training and validation accuracy suggests that the model is not overfitting, meaning it is learning the underlying patterns in the data rather than memorizing specific details that do not generalize well. The consistency across training and validation accuracies indicates that the model's predictions are reliable, making it suitable for real-world applications in melanoma detection.

###Class Rebalancing Impact:
The application of class rebalancing played a crucial role in improving the model's performance. Initially, the dataset had some class imbalances, where images of certain types of lesions (such as melanomas) were more abundant than others. Class rebalancing techniques, such as oversampling the minority class or undersampling the majority class, were employed to address this imbalance. This led to better training outcomes, especially in terms of improving the model's ability to recognize underrepresented classes and avoid bias toward the majority class. As a result, the model's accuracy on both classes (benign and malignant) has improved, making it more robust in distinguishing between melanoma and non-melanoma lesions.

###Loss Function:
The training loss of 0.7344 and validation loss of 0.6942 are reasonably low, which further indicates that the model is converging well and not overfitting. A lower validation loss relative to training loss typically signals that the model is not memorizing the training data but is instead learning generalizable features that can be applied to new, unseen data.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Technologies Used
- Pandas
- Numpy
- TensorFlow
- Keras
- Matplotlib
- Seaborn
- Augmentor

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
