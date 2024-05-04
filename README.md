  <h2 align="center">VigiLens: Deepfake Videos Detection Using Deep Learning</h2>
  <div align="center">
    VigiLens is a deepfake video detection model created using advanced deep learning techniques. 
    We're currently working on developing a user-friendly interface for the system.
  </div>

## 📋 <a name="table">Table of Contents</a>

1. 🤖 [Introduction](#introduction)
2. ⚙️ [Tech Stack](#tech-stack)
3. 🔋 [Features](#features)
4. 🗂️ [Directory Structure](#directory-structure)
5. 👩🏾‍💻 [Contributors](#contributers)
6. ❗ [Limitations & Future Scope](#limitations-&-future-scope)

## <a name="introduction">🤖 Introduction</a>

  **VigiLens** is a deepfake video detection model created using advanced deep learning techniques like RestNext and LSTM to 
  predict whether the given video is **Real or Fake(AI Synthesized)**. We implemented the model using a pre-trained ResNext CNN model to extract frame-level features and LSTM for temporal sequence
 processing to spot changes between the t and t-1 frame. This approach overcomes challenges faced by previous deepfake detection models, such as struggles with higher-resolution videos,
 data oversampling issues, and a lack of robustness. 
  We're currently working on developing a scalable user-friendly interface for the system.

## <a name="tech-stack">⚙️ Tech Stack</a>

- Python
- Libraries: Tensorflow, OpenCV, Pytorch, numpy, matplotlib, Face Recognition, pandas
- Django
  
## <a name="features">🔋 Features</a>

👉 **Dataset Diversity**: Comprehensive datasets with varied facial expressions, lighting, and scenarios.

👉 **Hybrid Model Architecture**: Integration of CNN and RNN for feature extraction and temporal analysis.

👉 **Optimized Training**: Adam optimizer, cross-entropy loss, and model fine-tuning.

👉 **Real-time Prediction**: Quick and accurate classification of videos as real or deepfake.

👉 **Confidence Metrics**: Providing confidence levels for classification results.

## <a name="directory-structure">🗂️ Directory Structure</a>

The directory Structure is given below:
```
Deepfake_detection_using_deep_learning
    |
    |--- Web Application
    |--- Deepfake Detection Model 
    |--- Documentaion
```
1. **Web Application** 
   - This directory will hold Web Application where a user can upload the video and submit it to the model for prediction. The trained model will perform the prediction and the result will be displayed on the screen.
2. **Deepfake Detection Mode**l 
   - It contains procedure of creating and training a deepfake detection model using our approach.
3. **Documentation**
   - It has related documentation done for the project.

##  <a name="contributers">👩🏾‍💻 Contributors</a>
- Sanskruti B.
- Trithi Amin
- Anusha Goyal
  
##  <a name="limitations-&-future-scope">❗ Limitations & Future Scope</a>

👉 **Upscaling to Browser Plugin/Web Application**: This project can be scaled up from a web-based platform to a browser plugin for automatic deepfake detection. Integration into large applications like WhatsApp and Facebook can provide convenient pre-detection capabilities for users, enhancing accessibility.

👉 **Expanding Detection Capabilities**: Although the current algorithm focuses on face deepfakes, there's room for improvement to detect full-body deepfakes. This enhancement would significantly increase the system's effectiveness and coverage, addressing broader deepfake scenarios.

👉 **Audio Detection Limitation**: Currently, the system is only capable of detecting videos without audio. Future enhancements may include audio analysis for more comprehensive deepfake detection.

##  🚀 Follow to see what we're building!
Have Suggestions? Want to colab? Shoot an [email](sanskrutib.dev@gmail.com)

``` Show some ❤️ by starring this repo! ⭐ ```
