# python-project: Pneumonia detection using deep learning
Open-source Pneumonia Detection system using Deep Learning.

Downloaded the dataset from Kaggle: https://www.kaggle.com/c/rsna-pneumonia-detection-challenge/data.

# Abstract
Pneumonia is an infection in one or both lungs. Bacteria, viruses, and fungi cause it. The infection causes inflammation in the air sacs in your lungs, which are called alveoli. In the proposed work an automated Pneumonia detection screening system is used to detect the severity of the disease. Medical images of patients' lungs of the format DICOM(dcm) are used for various pre-processing techniques, data visualization, and EDA. The model is built using a deep learning model. The model is tested and fine-tuned with different hyperparameters, by trying different optimizers, loss functions, epochs, learning rates, batch size, checkpointing, early stopping, etc.

# Introduction
Pneumonia is an infection in one or both lungs. Bacteria, viruses, and fungi cause it. The infection causes inflammation in the air sacs in your lungs, which are called alveoli. Pneumonia accounts for over 15% of all deaths of children under 5 years old internationally. It requires a review of a chest radiograph (CXR) by highly trained specialists and confirmation through clinical history, vital signs, and laboratory exams. Pneumonia usually manifests as an area or areas of increased opacity on CXR. However, the diagnosis of pneumonia on CXR is complicated because of a number of other conditions in the lungs such as fluid overload (pulmonary edema), bleeding, volume loss (or collapse), lung cancer, or post-radiation or surgical changes. Outside of the lungs, fluid in the pleural space (pleural effusion) also appears as increased opacity on CXR.CXRs are the most commonly performed diagnostic imaging study. A number of factors such as the positioning of the patient and depth of inspiration can alter the appearance of the CXR, complicating interpretation further. In addition, clinicians are faced with reading high volumes of images every shift. Now to detect Pneumonia we need to detect Inflammation of the lungs. Medical images are used to train and build models for Pneumonia detection.
In this project, we are building an algorithm to detect a visual signal for pneumonia in medical images. Specifically, the algorithm will automatically locate lung opacities on chest radiographs. There are various techniques and methodologies used in image processing and machine learning to identify abnormal digital images.


# Results and Analysis
We have trained three popular models and these are the analysis and result
| Modal                        | Accuracy  | 
| ---------------------------- | --------  |
| `Resnet Trained from scratch`|   81%     |                     
| `VGG19, pretrained`          |   70%     | 
| `Mobilenet`                  |   73%     |   
   

From the above table, it is clear that the proposed CNN resnet model trained from scratch we developed as part of this project gives us better accuracy.
Considering the model is built from scratch and we were able to achieve a decent accuracy. The below table shows results of the Model we developed :

| Accuracy Type         | Accuracy  | 
| --------------------- | --------  |
| `Training Accuracy`   |   97.16%  |
|` Validation Accuracy` |   83.91%  | 
| `Testing accuracy `   |   81.24%  | 

 Below are a few test images of our prediction algorithm in action, the Red box is the ground truth, the blue box is a prediction
 
   ![resmodelout](https://user-images.githubusercontent.com/13364936/156719726-b225da64-92b4-4a5f-819a-107e2616089f.PNG)
