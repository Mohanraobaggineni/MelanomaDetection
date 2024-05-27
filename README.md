# CNN Based Model To detect Melenoma
> This project uses a custom CNN to detect melanoma in images of skin lesions among 9 classes. 

## Table of Contents
* Melanoma-Detection-using-using-custom-cnn
    * Table of Contents
    * General Information
        * Algorithms Used
        * Dataset Information
    * Steps Involved
    * Results
        * Baseline Model
        * Augmented Model
        * Final Model
    * Conclusion
    * Acknowledgements
    * Technologies Used
    * Contact
   

<!-- You can include any other section that is pertinent to your problem -->

## General Information
This project focuses on developing a convolutional neural network (CNN) model for melanoma detection.
The background of the project lies in the significance of early detection of melanoma, a type of skin cancer that can be deadly if not diagnosed and treated promptly.
The business problem addressed by this project is the need for accurate and efficient detection of melanoma, which accounts for a significant portion of skin cancer deaths.
The dataset used in this project is obtained from the International Skin Imaging Collaboration (ISIC). It consists of images of various skin lesions, including melanoma, nevus, and other benign and malignant lesions, collected for the purpose of skin cancer research and diagnosis.

### Algorithm Used
Convolution Neural Network
     
### Dataset Information
The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed by the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.

The data set contains the following diseases:
* Actinic keratosis
* Basal cell carcinoma
* Dermatofibroma
* Melanoma
* Nevus
* Pigmented benign keratosis
* Seborrheic keratosis
* Squamous cell carcinoma
* Vascular lesion


### Steps Involved
* Data Loading
* Baseline Model Building
* Training the Model and testing the model (Addressing Overfitting,Addressing low accurachy,Addressing class imbalance)
* Building an augmented model
* Training the augmented model and testing the model
* Countering Class Imbalance with augmentor
* Building the final model
* Training the final model and testing the model
* Verifying the model

### Project Pipeline:
* Data Reading/Data Understanding
* Dataset Creation: Creating Train/Validation datasets
* Dataset visualisation: Visualizing one image per class
* Model building and training
* Addressing Overfitting
* Addressing low accurachy
* Addressing class imbalance
* Rerunning the model after making the above changes
* Visualizing the validation loss and accuracy

### Results
- Baseline Model
   Accuracy and Loss charts for the Base model
  ![Base_Model](Base_Model.png)
- Augmented Model
   Accuracy and Loss charts for the augmented model
  ![Aug_Model](Aug_Model.png)
- Final Model
       Accuracy and Loss charts for the final model
       ![Final Model](Final_Model.png)

 

## Conclusions
Addressed Overfitting
Addressed low accurachy
Addressed class imbalance

In conclusion, the project successfully developed a custom CNN model for melanoma detection using the ISIC dataset.

## Acknowledgements
Give credit here.

This project was inspired by upGrad


## Technologies Used
Google Colab
tensorflow 
Augmentor
matplotlib


<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Contact
Created by [@MohanRaoBaggineni] - feel free to contact me!
