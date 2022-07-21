# Textile-Defect-Detection
<h2>Introduction</h2>
Textile industry is one of the most thriving industries; but with the immense success ratio of this industry, there
are many other problems related to it - one of them being
the quality of the textile after every production step. There are
high possibilities of defects being caused due to machine defects,
faulty yarns, machine spoils and extreme stretching, etc. which
need to be looked for during the entire process. In this paper,
we look onto 5 different types of defects - colour defect, cuts,
holes, faulty threads, and metal contamination. Two different
methodologies have been used to understand and analyse these
defects through practical application by Fourier Analysis and
Mathematical Morphological methods which in turn determine
the quality of the textiles.


<h2>Data:</h2>

we have selected 5 images of each defected class(good,colour,hole,cut,mettalic contamination) and worked on them.

Method used:<br />
1)Textile Defect Detection using Fourier Transform<br />
2)Textile Defect Detection using Morphological operations

<h2>Dataset:</h2>

dataset Link:https://www.kaggle.com/datasets/belkhirnacim/textiledefectdetection

Dataset file to load images:
test32.h5



<h2>Approach 1:</h2>

<h3>Fourier transform :</h3>

Fourier transform is a salient Image Processing tool that is used to convert images into frequency domain. 
The spatial frequency directly relates with the brightness of the image. The magnitude of the sinusoid directly relates with the contrast.
The Fourier Transform is used in a wide range of applications, such as image analysis, image filtering, image reconstruction and image compression.


<h3>Implemenation:</h3>


Run the file Textile_Quality_Control.ipynb

#note keep the dataset and ipynb file in same folder

<h3>Breif:</h3>
The main approach that has been used for fabric defect detection is to perform fourier transformation on the given image and the threshold the image (or convert it to binary image).
After applying these operations on the image the defects in the fabric will be clearly visible in the histograms plotted
Here we have take 5 images from each category (good,colour,cut,holes and metallic contamination, thread),and and performed operation on them.


<h2>Approach2:<h2>


<h3>Morphology:</h3>

Morphology is a broad set of image processing operations that process images based on shapes. Morphological operations apply a structuring element to an input image, creating an output image of the same size.

<h3>Types of Morphological operations:</h3>

1)Dilation 
Morphological dilation makes objects more visible and fills in small holes in objects. Lines appear thicker, and filled shapes appear larger.

<br />2) Erosion
Morphological erosion removes floating pixels and thin lines so that only substantive objects remain. Remaining lines appear thinner and shapes appear smaller.

3)Open
Morphological opening is useful for removing small objects and thin lines from an image while preserving the shape and size of larger objects in the image

<br />4) Close
Morphological closing is useful for filling small holes in an image while preserving the shape and size of large holes and objects in the image.

<h3>Implementation:</h3>

Run the morphology (1).ipynb file
#note keep the dataset and ipynb file in same folder

<h2>Breif:</h2>

Here basically we have converted the input image into grey scale image and   equilized the image ,after that we have applied erosion on image which basically endances the backgroundor inhances spaces in he images ,and convert the eroded image toa binary image to see the textile defect properly.
<br />
You can also refer the research paper as well as the ppt for better understanding
