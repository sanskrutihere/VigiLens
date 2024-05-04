  <h2 align="center">Deepfake Detection Model 🤖 </h2>
  <div align="center">
   This process involves collecting diverse datasets, preprocessing videos by importing, cropping, and creating uniform frames, training a PyTorch model using transfer learning with RestNext50 and LSTM, and finally predicting video authenticity with confidence using the trained model.
  </div>
  
## ⚙️ Recommended Tools:
Google Colab, Jupyter Notebook

## 📋 <a name="table">Table of Contents</a>

1. [Dataset Collection](#DatasetCollection)
2. [Preprocessing](#Preprocessing)
3. [Training](#Training)
4. [Prediction](#Prediction) 

## <a name="DatasetCollection">🐍 Dataset Collection:</a>
- Celeb DF v2 datasets offer large volumes of celebrity videos with varied deepfake variations.
- FaceForensics dataset includes over 500,000 frames from YouTube videos, suitable for researching image or video forgeries.
- Both datasets provide rich deepfake instances with different manipulation techniques and realism levels, aiding in robust model training and evaluation.
The datasets we used are listed below:
  - [FaceForensics++](https://github.com/ondyari/FaceForensics)
  - [Celeb-DF](https://github.com/yuezunli/celeb-deepfakeforensics)
Here's Snippet of our dataset!
<p align="center">
  <img src="https://github.com/sanskrutihere/VigiLens/blob/main/Deepfake%20Detection%20Model/assets/Dataset.png" />
</p>

## <a name="Preprocessing">🐍 Preprocessing:</a>
- Imported all videos into a Python list using glob.
- Used cv2.VideoCapture to read videos and determine mean frames, selecting 150 frames for uniformity.
- Split videos into frames and cropped to face location.
- Created new video with 112 x 112 resolution at 30 frames per second in mp4 format.
- Used first 150 frames for LSTM temporal sequence analysis.
- Labels for above preprocessed data is under `/label/Global_metadata.csv`

## <a name="Training">🐍 Training:</a>
  - It will load the preprocessed video and labels from a csv file.
  - Create a pytorch model using transfer learning with RestNext50 and LSTM.
  - Split the data into train and test data
  - Train the model
  - Test the model
  - save the model in .pt file
    
## <a name="Prediction">🐍 Prediction:</a>
  - Load the saved pytorch deepfake detection model
  - Predict the output whether the video is real or fake, along with the confidence of the prediction.
<p align="center">
  <img src="https://github.com/sanskrutihere/VigiLens/blob/main/Deepfake%20Detection%20Model/assets/Prediction.png" />
</p>
  
