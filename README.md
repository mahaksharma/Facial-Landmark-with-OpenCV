# Facial-Landmark-with-OpenCV with Viola Jones alternate solution link
Solution1:
The facial Landmark detection using OpenCV.
Facial landmarks with dlib, OpenCV, and Python
Facial landmarks are used to localize and represent salient regions of the face, such as:

Eyes
Eyebrows
Nose
Mouth
Jawline

Facial landmarks have been successfully applied to face alignment, head pose estimation, face swapping, blink detection and much more.
Facial landmarks are used to label and identify key facial attributes in an image (source).

Detecting facial landmarks is a subset of the shape prediction problem. Given an input image (and normally an ROI that specifies the object of interest), a shape predictor attempts to localize key points of interest along the shape.

In the context of facial landmarks,goal is detect important facial structures on the face using shape prediction methods.

Detecting facial landmarks is therefore a two step process:

Step #1: Localize the face in the image.
Step #2: Detect the key facial structures on the face ROI.
Face detection (Step #1) can be achieved in a number of ways.

Given the face region we can then apply Step #2: detecting key facial structures in the face region.

There are a variety of facial landmark detectors, but all methods essentially try to localize and label the following facial regions:

Mouth
Right eyebrow
Left eyebrow
Right eye
Left eye
Nose
Jaw
This method starts by using:

A training set of labeled facial landmarks on an image. These images are manually labeled, specifying specific (x, y)-coordinates of regions surrounding each facial structure.
Priors, of more specifically, the probability on distance between pairs of input pixels.
----------------------------------------------
Solution 2:
I've added my alternate solution of using Viola Jones algorithm for face detection and recognition which is own research paper work implementation.Basically landmark features are categorised as Haar features(facial) to recognise any face.The algorithm was trained on various face and non face dataset and Adaptive Boosting/Cascading is used to extract out relevant features to detect a face.For further information

Viola jones github repo link:

https://github.com/mahaksharma/Viola-Jones-Face-Detection-Algorithm

