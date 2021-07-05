# human_recognition
- Keras MobileNetV2 [model](https://drive.google.com/drive/folders/1-OPoMEf7xdRtCo0M9WiV0G8dgfUeAqu6?usp=sharing), which is trained to respond if there are people in the image.
- A [dataset](https://drive.google.com/file/d/13AJu4DOpMVd15DPi6ZflJpdxx37Lpctw/view?usp=sharing) on which it trained.

  The train dataset contains 2500 images with people and 2500 images without people. Most of the images contain scenes such as apartments, streets, nature, etc. Validation dataset contains 500/500 images with/without people.
  
  The model is MobileNetV2 from Keras applications, with GlobAveragePooling and 2 Dense layers at top. The model input has the shape (512, 512, 3), with values in range [-1. 1]. The output contains two classes: a class of images with people and a class of images without.
  
  The best validation accuracy is 0.9526.
