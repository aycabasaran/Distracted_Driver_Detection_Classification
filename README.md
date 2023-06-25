# 🚗 Image Classification: Distracted Driver Detection 🚗 


### 🎯 **Overview**

In this project, I utilize machine learning models to classify images of drivers engaged in various activities. The dataset comprises images of drivers performing different actions such as texting, eating, talking on the phone, makeup, reaching behind, and more. The goal is to predict the driver's action in each picture accurately.

The 10 classes to predict are:

- 🚗 c0: safe driving 
- 📱 c1: texting - right 
- ☎️ c2: talking on the phone - right 
- 📱 c3: texting - left 
- ☎️ c4: talking on the phone - left 
- 🎵 c5: operating the radio 
- 🥤 c6: drinking 
- 👋 c7: reaching behind 
- 💄 c8: hair and makeup 
- 👥 c9: talking to passenger


### 🔧 **Technology Stack**

Python, Tensorflow, Keras, Pandas, NumPy, Scikit-Learn, Matplotlib.


### 💡 **Methodology**

The methodology for this project involved developing and comparing a custom-built Convolutional Neural Network (CNN), a VGG16 model and a MobileNetV2 model. 


**Custom CNN Model**:
- Architecture: Custom CNN
- Batch Size: 100
- Optimizer: Adam
- Learning Rate (α): 0.001


**VGG16 Model with Image Augmentation**:
- Pre-trained Model: VGG16
- Batch Size: 60
- Optimizer: Adam
- Learning Rate (α): 0.005
- Data Augmentation: Yes


**MobileNetV2 Model with Hyperparameter Tuning and Image Augmentation**:
- Pre-trained Model: MobileNetV2
- Batch Size: 120
- Optimizer: SGD
- Learning Rate (α): 0.003
- Data Augmentation: Yes


### 💭 **Main Conclusions**

From the above models, it was clear that each approach had its own strengths and weaknesses. While the Custom CNN model served as a good starting point, the transfer learning models (VGG16 and MobileNetV2) demonstrated superior performance. However, these models aren't perfect and can be further optimized. Here are some improvements that can be made:

- 🎛️ Refine Data Augmentation: Data Augmentation was beneficial but introduced some noise in the images, which could potentially impact the model's performance
  
- ⏱️ Adjust Learning Rate and Increase Epochs: Tuning the learning rate and increasing the number of epochs could potentially improve the model's accuracy
  
- 🔧 Implement Advanced Hyperparameter Tuning Techniques: Techniques like Grid Search or Random Search can be employed to explore many combinations of parameters systematically and find the best performing ones
