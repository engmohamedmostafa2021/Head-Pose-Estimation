*Head Pose Estimation*

Head Pose estimation is a computer vision technique to track the movements of a person's Face This is usually performed by finding the location of key points for the given objects. Based on these key points we can compare various movements and postures and draw insights. Pose estimation is actively used in the field of augmented reality, animation, gaming, and robotics.


![head](https://github.com/engmohamedmostafa2021/Head-Pose-Estimation/blob/main/Final%20with%20Angles.gif)


- In this project we will draw the 3 position axis (pitch,yaw,roll) by predicting the 3 angels of each position by training 3 models to predict each angel. 
- We will use [AFLW2000](http://www.cbsr.ia.ac.cn/users/xiangyuzhu/projects/3DDFA/Database/AFLW2000-3D.zip) dataset with contains 2000 image and 2000 matlab file with contains the 3 labels (angels).
- We will use MediaPipe library in both training and testing phases:
  - In Training: first we dtect the face of each image then using the same library to generate the landmark points of the face after this phase the training data (features) will contain 1853 samples with 936 columns (468 for X and 468 for Y), for labels we will extract the 3 angels from the mat file. 
  - In Testing: we will use the MediaPipe Library to generate the landmarks as we did in the training phase and using the trained models to predict the 3 labels and using them to draw the axis.  

## Steps of the notebook:
    - 1. Importing Libraries. 
    - 2. Loading Data. 
    - 3. Preparing the data for Training.
    - 4. Prpcessing the Data.
    - 5. Splitting the data for training the model and validation.
    - 6. GridSearch for XGBoostRegressor and SVR models.
    - 7. Defining function for drawing the 3 axis.
    - 8. Drawing the axis from the true labels on the image.
    - 9. Testing the model on the image.
    - 10. Testing the model on a video by processing its frames and drawing the axis on them.

## 🛠 Skills
Deep Learning, Computer Vision, Python, TensorFlow, OpenCV...


## 🔗 Links
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/muhamedmustafa/)

