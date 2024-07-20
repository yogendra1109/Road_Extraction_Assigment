# Road_Extraction_Assigment

Task for Interview

There are 2 classes (basically a binary image segmentation task).
This is a part of computer vision task.
**Data Handling and Preprocessing
First, the original data is loaded.
The training data (masks) are successfully binarized.
The image sets (train, valid, test) are resized to the size of (256, 256, 3). This is to make sure the sizes of the images are same.
Whole data is saved in the drive to avoid continuous repetition of code execution.**
**Model Architecture
U-Net: Implemented a U-Net architecture, which is well-suited for image segmentation tasks.
Encoder: Consists of multiple convolutional blocks with downsampling.
Bridge: Connects the encoder and decoder with the highest level features.
Decoder: Upsamples the features and combines them with corresponding encoder features for precise segmentation.**
**Model Training
Data Augmentation: Used horizontal and vertical flipping to augment the training data and improve model generalization.
Training Strategy:
Split the training data to create a custom validation set.
Used ModelCheckpoint to save the best model based on validation accuracy.
Compiled the model with the Adam optimizer and binary cross-entropy loss function.**
**Results and Future Work
The model demonstrated good performance in extracting roads from satellite images, with visual inspections confirming accurate road delineation.
Future work could involve experimenting with more advanced augmentation techniques, tuning hyperparameters, and exploring different architectures to further enhance model performance. Due to GPU issue the model lacks in few visulaisation, With GPU support Model can Perform really well.
Reference Are- Kaggle, ChatGPT
https://www.kaggle.com/code/balraj98/road-extraction-from-satellite-images-deeplabv3
