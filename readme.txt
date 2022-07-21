Topic:
Textile Quality Control with Image Processing Techniques

Motivation:
The textile industry undergoes several steps of production before the final product reaches the market. 
And with each step the quality of the product needs to be reassured. 
As human visual inspection of the same could be very time consuming and could delay the production of the same.


Objective:

Our objective is to use image processing techniques to identify the defects and assure the quality of the textile.


Data:

we have selected 5 images of each defected class(good,colour,hole,cut,mettalic contamination) and worked on them.

Method used:
1)Textile Defect Detection using Fourier Transform
2)Textile Defect Detection using Morphological operations

Dataset:

dataset link:Link:https://www.kaggle.com/datasets/belkhirnacim/textiledefectdetection

Dataset file to load images:
test32.h5



Approach 1:

Fourier transform :

Fourier transform is a salient Image Processing tool that is used to convert images into frequency domain. 
The spatial frequency directly relates with the brightness of the image. The magnitude of the sinusoid directly relates with the contrast.
The Fourier Transform is used in a wide range of applications, such as image analysis, image filtering, image reconstruction and image compression.


Implemenation:


Run the file Textile_Quality_Control.ipynb

#note keep the dataset and ipynb file in same folder

Breif:
The main approach that has been used for fabric defect detection is to perform fourier transformation on the given image and the threshold the image (or convert it to binary image).
After applying these operations on the image the defects in the fabric will be clearly visible in the histograms plotted
Here we have take 5 images from each category (good,colour,cut,holes and metallic contamination, thread),and and performed operation on them.


Approach2:


Morphology:

Morphology is a broad set of image processing operations that process images based on shapes. Morphological operations apply a structuring element to an input image, creating an output image of the same size.

Trpes of Morphological operations:

1)Dilation 
Morphological dilation makes objects more visible and fills in small holes in objects. Lines appear thicker, and filled shapes appear larger.
2) Erosion
Morphological erosion removes floating pixels and thin lines so that only substantive objects remain. Remaining lines appear thinner and shapes appear smaller.

3)Open
Morphological opening is useful for removing small objects and thin lines from an image while preserving the shape and size of larger objects in the image
4) Close
Morphological closing is useful for filling small holes in an image while preserving the shape and size of large holes and objects in the image.

Implementation:

Run the morphology (1).ipynb file
#note keep the dataset and ipynb file in same folder

Breif:

Here basically we have converted the input image into grey scale image and   equilized the image ,after that we have applied erosion on image which basically endances the backgroundor inhances spaces in he images ,and convert the eroded image toa binary image to see the textile defect properly.


--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------