# Music Genre Classification
#### Team Members: Eslim Rana Emiroğlu, Betül Doğrul, Sefa Emre Kavgacı, Mehmet Kutay Buyruk, Muhammet Bahadır Mutlu
### Introduction:
This project investigates music genre classification using two distinct strategies. In the first part, we focus on audio classification by leveraging pretrained models for feature extraction, fine-tuning these models on our dataset, and training a model from scratch. The second part reframes the problem as an image classification task, where audio is converted into mel-spectrograms, and state-of-the-art image classifiers are applied to these representations. 
### Dataset:
Primary Dataset: Free Music Archive (FMA) dataset. The dataset consists of music tracks labeled by genre. We will use the "FMA Small" subset, which includes 8,000 MP3 tracks across 8 genres (1,000 per genre). This dataset was chosen for its size, diversity, and structured organization.
### Methodology:
#### Audio Classification:
- **Preprocessing**: Audio files are standardized by normalizing the sampling rate and cropping/padding duration. MFCCs, Chroma will be used for feature extraction. 
- **Machine Learning Models**: Random Forest and SVM will be used for classification.
- **Transfer Learning**: Pre-trained models such as VGGish, YAMNet, or OpenL3 will be fine-tuned on the audio files.
#### Image Classification:
- **Preprocessing**: Audio files will be converted into mel-spectrogram images, and some image preprocessing will be applied (normalization etc.)
- **CNN From Scratch**: Develop a convolutional neural network (CNN) directly on mel-spectrogram representations. Can compare benefits of transfer learning versus custom models.
- **Transfer Learning**: Pretrained models such as VGG16, ResNet50, and InceptionV3 will be fine-tuned on the spectrogram images.
### Evaluation & Comparison:
In the end, all approaches will be compared according to their final metrics, such as accuracy and F1-Score.
