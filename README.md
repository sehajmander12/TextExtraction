# Text-Extraction #

Project - 1 <br>

## Overview: ##
In this project, I have worked on extracting text from images. After extracting the text we will apply some basic functions of OpenCV on that text to enhance it and to get more accurate results. This project will be very useful as it will save time and effort of typing from an image.

### Live Link: https://text-extraction-application.herokuapp.com/ ###

### I/O Screenshot :<br/> ###
#### Input-1 (Original) ####
![](https://github.com/sehajmander12/TextExtraction/blob/main/sample_data/maya-angelou.png)

Output-1
![](https://user-images.githubusercontent.com/48948891/133932650-c126736b-77b7-4377-8e77-d755f3d939ba.png)
</br>
#### Input-2(Tampered) ####
![](https://user-images.githubusercontent.com/48948891/133932765-19ee7aed-168e-4e10-b9f2-1ce5f4501c3f.jpg)

Output-2
![](https://user-images.githubusercontent.com/48948891/133932696-8274d7ad-19ba-47f5-b7bb-55c73b9046b0.png)
</br>
### Summary :<br/> ###

-Finding out structural similarity of the images helped us in finding the difference or similarity in the shape of the images. Similarly, finding out the threshold and contours based on those threshold for the images converted into grayscale binary also helped us in shape analysis and recognition.<br>

-As, our SSIM is ~28.5% we can say that the image user provided is fake or tampered.<br>

-Finally we visualized the differences and similarities between the images using by displaying the images with contours, difference and threshold.<br>

### Novelty :<br/> ###
●	This project can be used in different organizations where customers or users need to provide any kind of id in order to get themselves verified.<br>

● The organization can use this project to find out whether the ID is original or fake. Similarly this can be used for any type of ID like adhar, voter id, etc.<br>

