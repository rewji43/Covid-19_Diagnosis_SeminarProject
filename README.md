# An Application of Machine Learning Techniques for Covid-19 Diagnosis <br>

Use CNN Architecture for Build Covid-19 Classification Model from X-ray Images and this project is on going <br>

## Data Info
 * Covid data from this Github : [covid](https://github.com/ieee8023/covid-chestxray-dataset)
 * Normal data from this Kaggle : [normal](https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia) <br>
 
 Covid data have 930 images but can use only 867 images when compare with metadata <br>
 Normal data have 1341 images, I use only normal case in Pneumonia Data set <br>

## Data Pre-processing
 
 First, I random choice images of normal to 867 images for avoid imbalance class and split train test 70:30 <br>
 and use pickle for save images data to pickle files, it can save images data and didn't change it when load again. <br>
 | Dataset   | Covid-19 | Normal | Total |
 | --------  | -------- | ------ | ----- |
 | Training  |    607   |  607   |  1214 |
 | Testing   |    260   |  260   |  520  |
 | Total     |    867   |  867   |  1734 |
 
 After I already complete with training and testing data, I follow these processes below <br>
 * Image Augmentation
 * Image Enhancement
 * Image resizing
 * Normalization

 
 * Image Augmentation
 Augmentation with rotate, crop and filp images and get new data set in this table <br>
 
 | Dataset   | Covid-19 | Normal | Total |
 | --------  | -------- | ------ | ----- |
 | Training  |    3035  |  3035  |  6070 |
 | Testing   |    260   |  260   |  520  |
 | Total     |    3295  |  3295  |  6590 |
 
 * Image Augmentation 
 I assumed histogram equalization will help a little bit then I try to use it
   
 * Image resizing
 In this project, I resize it into 400*400 because images in data set have various size.
 
 * Normalization
 I try to use data/ 255.0 in this project.

## Building Model
 
## Some Propose Model
 This project is on going but follow this link for some model completely : [sharing model](https://drive.google.com/drive/folders/1PohYcNMkky6X1F_luz3Av6wWWR0fGvW5)