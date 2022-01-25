# Face-Mask-Overlay-and-Face-Crop

The notebook in the repository is divided into two parts:-

## 1. Cropping facial region
In this i used dlib's get_frontal_face_detector funtion which then returns list of coordinates of the bounding box over the detected faces in an image. Here is the result:- 

<img src="/results/faceCrop.jpg">
<br>

## 2. Mask Overlay
In this i used dlib's facial landmark detector, which basically detects 68 landmark points on human face which covers face regions such as eyes, eyebrows, mouth, nose and jawline. 
You can find their visualization below:- 
<img src="/images/facial_landmarks_68markup-768x619.jpg">
<br>

Then by using opencv's findHomography funtion to find transform between matched keypoints, we get a new mask image in which the mask is mapped to the desired landmark points.
Here are the results:-

<img src="/results/mask3m.jpg">

<img src="/results/maskAntiCovid.jpg">

<img src="/results/maskWhiteMask.jpg">

### Requirements to run the notebook:-
1. Open CV
2. Dlib
3. PIL

### Credits:-
Github Repository:-
1. https://github.com/ID56/Fast-Face-Mask-Overlay (for masks annotation files)

Tutorial blogs:-
1. https://learnopencv.com/using-facial-landmarks-for-overlaying-faces-with-masks/

Dataset Used:-
1. https://www.kaggle.com/jessicali9530/celeba-dataset



