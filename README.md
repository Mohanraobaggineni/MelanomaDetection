# CNN based Melanoma Detection Model
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

###Project Pipeline:
Data Reading/Data Understanding
Dataset Creation: Creating Train/Validation datasets
Dataset visualisation: Visualizing one image per class
Model building and training
Addressing Overfitting
Addressing low accurachy
Addressing class imbalance
Rerunning the model after making the above changes
Visualizing the validation loss and accuracy

### Results
- Baseline Model
 Observations:

Training Loss and Accuracy:
Training Loss: 0.4190
Training Accuracy: 0.8311 (83.11%)

Validation Loss and Accuracy:
Validation Loss: 3.8681
Validation Accuracy: 0.4153 (41.53%)


Interpretation:

High Training Accuracy:
The model is performing well on the training data, achieving a high accuracy of 83.11%.

High Validation Loss:
The validation loss is significantly higher than the training loss. A high validation loss compared to training loss often indicates overfitting, where the model learns the training data well but fails to generalize to unseen validation data.

Low Validation Accuracy:
The validation accuracy is considerably lower than the training accuracy. This further supports the indication of overfitting.


Action items:
- Add Dropouts after initial convolution layers as well
- do - Data augmentation - Image rotation, Image flip, Image zoom




 
 
 
- Augmented Model
Observations:

Training Loss and Accuracy:
Training Loss: 1.2133
Training Accuracy: 0.5638 (56.38%)

Validation Loss and Accuracy:
Validation Loss: 2.3579
Validation Accuracy: 0.3559 (35.59%)

Interpretation:

Moderate Training Accuracy:
The training accuracy is 56.38%, indicating the model has improved its ability to learn from the training data but still shows room for improvement.

Low Validation Accuracy:
The validation accuracy is 35.59%, which is significantly lower than the training accuracy. This suggests that the model might be overfitting the training data, meaning it performs well on the training data but fails to generalize to the validation data.

High Validation Loss:
The validation loss is quite high (2.3579), which further indicates overfitting. High validation loss compared to training loss often suggests the model is not generalizing well.

1. We can see that though the accuracy hasn't improved greatly, overfitting has reduced
2. reasons could be image Augmentation, class imbalance
3. to reduce the overfitting further we could use batch normalization

Points 2 and 3 can be addressed using Image Augmentation







- Final Model
    Improved Accuracy and Reduced Overfitting:
The training accuracy of 90.38% and validation accuracy of 83.42% indicate significant improvements in the model's performance.
The validation loss of 0.6864 is notably lower than previous results, suggesting that the model is generalizing better to unseen data.

Reasons for Improved Performance:

Class Balancing: By addressing class imbalances, the model is now able to learn more effectively from each class, leading to better overall performance and reduced bias towards majority classes.

Batch Normalization: Normalizing the activations within each batch has stabilized and accelerated training, resulting in better convergence and reduced overfitting.

 

## Conclusions

##Model Improvement Process and Observations

Initial Model (No ImageDataGenerator)
Observation:
The model overfitted the data with a high ratio. This means the training accuracy was high, but the validation accuracy was significantly lower, indicating poor generalization to new data.





Adding Dropout and ImageDataGenerator

Dropout: Introduced dropout layers after initial convolution layers to randomly drop units and prevent overfitting.
ImageDataGenerator: Applied image augmentation techniques such as rotation, flipping, and zooming to artificially expand the training dataset and provide more diverse training examples.

Observation:
The addition of dropout and image augmentation reduced overfitting. The validation accuracy improved and became closer to the training accuracy, showing better generalization.






Adding Batch Normalization and Further Augmentation

Batch Normalization: Added batch normalization layers to normalize the activations within each batch, which helped stabilize and accelerate the training process.
Further Augmentation: Applied additional data augmentation techniques to further increase the diversity of training data.
Class Balancing: Ensured balanced representation of all classes in the training dataset to reduce bias towards majority classes.

Observation:
The introduction of batch normalization and further data augmentation significantly improved the model's performance. The validation accuracy was much closer to the training accuracy, indicating that the model was generalizing well.
The final metrics showed a training accuracy of 90.38% and a validation accuracy of 83.42%, with reduced validation loss, confirming the effectiveness of the changes.


In conclusion, the project successfully developed a custom CNN model for melanoma detection using the ISIC dataset.



## Technologies Used
Google Colab
TensorFlow Version: 2.15.0
Matplotlib Version: 3.7.1
Augmentor-0.2.12


<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Contact
Created by [@MohanRaoB] - feel free to contact me!
