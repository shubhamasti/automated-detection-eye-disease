# Automated and Explainable Detection of Multiple Diseases from Retinal Fundus Images

Training and testing code for automated and explainable detection of Pathological Myopia, Glaucoma and Diabetic Retinopathy.

## 1. Diabetic Retinopathy (DR)

test.ipynb: Test out the performance for detection and grading of DR on DDR and IDRiD datasets.

### a. Deep Learning
Contianes files related to deep learning approach for classification and grading.
- pretrained_tf.ipynb: Detection and grading of DR using pretrained models (from keras)
- gradcam.ipynb: Visualise regions of interest using Gradcam/Gradcam++

### b. Feature Based
Contianes files related to feature based approach for classification and grading.
- augment_SE.ipynb: Augment soft exudate images and masks
- classify_features.ipynb: Detection and grading of DR using segmented features
- test_segmentation.ipynb: Check performance of segmented features
- unet_EX.ipynb: Segmentation of hard exudates
- unet_HE.ipynb: Segmentation of haemorrhage
- unet_MA.ipynb: Segmentation of microaneurysms
- unet_SE.ipynb: Segmentation of soft exudates

### c. models_features
Saved models (json and weights) of the CNN used to classify and grade DR from features.

### d. models_segmentation
Saved segmentation models (json and weights) of the features of DR (EX, HE, MA, SE).

### e. models_TL
Saved transfer learning based models (json and weights) used to classify and grade DR.


## 2. Glaucoma

test_classify.ipynb: Test out the perofrmance for detection of Glaucoma on REFUGE and ORIGA datasets.

### a. Feature Based
Contianes files related to feature based learning approach for detection of glaucoma.
- classify_features.ipynb: Presence of glaucoma using segmented features
- ODOC.ipynb: Segmentation of optic disc and cup
- test_segmentation.ipynb: Check performance of segmented features

### b. models_features
Saved models (json and weights) of the CNN used to detect glaucoma from features.

### c. models_segmentation
Saved segmentation model (json and weights) of the features of glaucoma (optic disc and cup).


## 3. Pathological Myopia (PM)

test_classify.ipynb: Test out the perofrmance of detection of PM on PALM dataset.

### a. Deep Learning
Contianes files related to deep learning approach for detection of pathological myopia.
- pretrained_tf.ipynb: Presence of PM using pretrained models (from keras)
- gradcam.ipynb: Visualise regions of interest using Gradcam/Gradcam++

### b. Feature Based
Contianes files related to feature based learning approach for cdetection of pathological myopia.
- classify_features.ipynb: Detection of PM using segmented features
- test_segmentation.ipynb: Check performance of segmented features
- unet_atrophy.ipynb: Segmentation of retinal atrophy
- unet_OD.ipynb: Segmentation of optic disc

### c. models_features
Saved models (json and weights) of the CNNs used to detect PM from features.

### d. models_segmentation
Saved segmentation models (json and weights) of the features of PM (retinal atrophy, optic disc).

### e. models_TL
Saved transfer learning based models (json and weights) used to detect PM.
