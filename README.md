# Udacity-ML_CV-Project
This is my project for Udacity Self Driving Cars Nano Degree First Module ML_CV

Find tensorboard values in each model folder

# Goal
To have high mAP above 0.45
No Overfitting or Underfitting occur

#Experiment
Training the three models 

Starting with the EfficientDet D1 640x640 to have acceptable loss for training and eval of 0.4,0.5 poor for DetectionBoxes_Percision/mAP with 0.1 value

Then I started SSD ResNet50 V1 FPN 640x640 (RetinaNet50) model with so promising expectations as I read before that ResNet is one of the best detection models but due to bad choose for hyperparameters I had training loss of 0.5 and evaluation loss of 0.95 and that indicates that I am having Overfitting due to bad selection of parameter

Learning from my mistakes at ResNet50 model and starting SSD MobileNet V2 FPNLite 640x640 model training to have better values but not the best for loss of training with for training 0.95 and evaluation of 0.96 well no overfitting but still very poor performance due to either poor choice of model architecture or incorrect hyperparameters but having higher values for mAP than ResNet and better state for video output

To improve the performance i will need better hyperparameters tuning for the values I used and may increase training steps for some models and sure add some data augmentation to the data input

#Choise
In my case I had the best performace but still poor from SSD MobileNet V2 FPNLite 640x640 model it will be acceptable in some cases but not for self driving cars as this case is critical but it still fastest to implement and deploy but for future work I will improve SSD ResNet50 V1 FPN 640x640 (RetinaNet50) hyperparameters tuning to avoid overfitting and with so improvements this case will be the best
