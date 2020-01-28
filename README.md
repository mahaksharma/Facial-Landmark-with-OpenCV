# Facial-Landmark-with-OpenCV along with Viola Jones alternate solution link
Solution1:
The facial Landmark detection using dlib, OpenCV, and Python
Facial landmarks are used to localize and represent salient regions of the face, such as:

1.Eyes
2.Eyebrows
3.Nose
4.Mouth
5.Jawline

Applications: 
1.Facial landmarks have been successfully applied to face alignment, head pose estimation, face swapping, blink detection and much more.

2.Facial landmarks are used to label and identify key facial attributes in an image (source).

Detecting facial landmarks is a subset of the shape prediction/recognition problem. Given an input image (and normally an ROI that specifies the object of interest), a shape predictor attempts to localize key points of interest along the shape.

In the context of facial landmarks,my goal is detect important facial structures on the face using shape prediction methods.

Detecting facial landmarks is therefore a two step process:

Step #1: Localize the face in the image.
Step #2: Detect the key facial structures on the face ROI.
Face detection (Step #1) can be achieved in a number of ways.

Given the face region we can then apply 
Step #2: detecting key facial structures in the face region.

There are a variety of facial landmark detectors, but all methods essentially try to localize and label the following facial regions:

1.Mouth
2.Right eyebrow
3.Left eyebrow
4.Right eye
5.Left eye
6.Nose
7.Jaw
This method starts by using:

1.A training set of labeled facial landmarks on an image. These images are manually labeled, specifying specific (x, y)-coordinates of regions surrounding each facial structure.
2.Priors, of more specifically, the probability on distance between pairs of input pixels.

Given this input data, an ensemble of regression trees are trained to estimate the facial landmark positions directly from the pixel intensities themselves (i.e., no “feature extraction” is taking place).

The end result of my solution is a facial landmark detector that can be used to detect facial landmarks in real-time with high quality predictions.

----------------------------------------------

Solution 2:
I've added my alternate solution of using Viola Jones algorithm for face detection and recognition which is own research paper work implementation.Basically landmark features are categorised as Haar features(facial) to recognise any face.The algorithm was trained on various face and non face dataset and Adaptive Boosting/Cascading is used to extract out relevant features to detect a face.For further information

Viola jones github repo link:

https://github.com/mahaksharma/Viola-Jones-Face-Detection-Algorithm

