# ML-Sign-Language-Detection-

We took our research paper as https://www.irjet.net/archives/V7/i3/IRJET-V7I3418.pdf

The motivation behind this project is to provide a platform for the deaf community to be able to converse with those who do not know sign language. Our sign language detection system will help to identify certain hand movements as English words in correspondence with ASL American Sign Language and ISL Indian Sign Language. 
Since we are dealing with a relatively unique dataset, part of our project involved making our own data and preprocessing and feature extraction.
This was followed by applying the Machine Learning Algorithm used in the research paper chosen.

## Image Frame Acquisition and Image Capture
Using OpenCV we first set up the frame to capture the images and video for real time sign language detection

![image](https://user-images.githubusercontent.com/73610600/164746274-0a9ef5db-b235-4bec-a231-f39d870aa4c6.png) 

## Image Segmentation
With respect to Classification, we need to segment the skin part of the image first and regard the remaining part as noise. We performed training on the Skin Segmentation dataset from the University of California Irvine database.

![image](https://user-images.githubusercontent.com/73610600/164747065-e3296bb2-035d-43e6-969b-eb90fd5d6134.png)

## Feature Extraction
A simple way to perform feature extraction is to use SIFT(Scale Inverse Feature Transform)features as it registers key points rather than finding the features manually.

![image](https://user-images.githubusercontent.com/73610600/164747187-36375b08-2936-4630-b70a-473cfab12490.png)

## Algorithm
We will be using SVM classifier (SVC) which are capable of performing linear classifications as well as non-linear classifications using kernels. We will be using a gaussian kernel for this classification. Here we are using 20% of dataset as testset.

![image](https://user-images.githubusercontent.com/73610600/164747309-c0e01f6e-a0b4-4ec6-90fc-f56bb26e84b2.png)

Classification report shows accuracy (~ 93%) 
Macro avg (precision 92% recall 91% f1-score 93% support 110)


