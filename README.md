# Text-Extraction #

Project - 1 <br>

## Overview: ##
In this project, I have worked on extracting text from images. After extracting the text we will apply some basic functions of OpenCV on that text to enhance it and to get more accurate results. This project will be very useful as it will save time and effort of typing from an image.

## Methedology of the Extractor ##
![Screenshot 2021-09-20 at 9 12 15 PM](https://user-images.githubusercontent.com/60060524/134031619-392ce018-6bd8-4d23-80e6-2e45c7b642b8.png)</br>
Here we can see the procedure that we've followed to extract text out of an complex image, we can see these in the collab notebook as well. </br>
●	I start with importing the required packages.</br>
●	I use teserract to extract the text and remove all the irrelevant symbols from characters.</br>
●	Then we read the image into opencv format to process it further. This is required when I need to extract the text from complex images.</br>
●	Then I convert the images to grayscale so that it becomes less complex to process.</br>
●	This is followed by blurring the image so that we can remove the noise from the image.</br>
●	After this I performed threshold transformation. If pixel value is greater than a threshold value, it is assigned one value (may be white), else it is assigned another value (may be black). </br>
●	Erode transformation is done. cv2.erode() method is used to perform erosion on the image. The basic idea of erosion is just like soil erosion only, it erodes away the boundaries of foreground object (Always try to keep foreground in white). </br>
●	Performed morphological trandformation which is used in opening small holes inside the foreground objects, or small white points on the object.
●	Canny transformation is used to detect egdes in the image. </br>
●	Applied deskewing on the image. Deskewing is a process whereby skew is removed by rotating an image by the same amount as its skew but in the opposite direction. This results in a horizontally and vertically aligned image where the text runs across the page rather than at an angle.</br>
Generally, since we don't come accross very complex images we can extract text out of images using teserract after preproccessing.</br>
### Live Link: https://text-extraction-application.herokuapp.com/ ###

### I/O Screenshot :<br/> ###
#### Input-1  ####
![maya-angelou](https://user-images.githubusercontent.com/60060524/134026698-76884845-c784-4cdb-8aa7-3a9cfb39a202.png)


Output-1
![Screenshot 2021-09-20 at 8 34 12 PM](https://user-images.githubusercontent.com/60060524/134026764-d04d07d1-4885-405f-a820-f3dbe340ddeb.png)
</br>

#### Input-2 ####
![Forty Rules](https://user-images.githubusercontent.com/60060524/134027188-4029365f-7ec3-41c5-b8a9-ff64f50353ee.png)



Output-2
![Screenshot 2021-09-20 at 8 33 58 PM](https://user-images.githubusercontent.com/60060524/134026941-0d09112c-39ca-45e5-9c17-67f6bb8f77aa.png)
</br>

### Summary :<br/> ###

-Finding out structural similarity of the images helped us in finding the difference or similarity in the shape of the images. Similarly, finding out the threshold and contours based on those threshold for the images converted into grayscale binary also helped us in shape analysis and recognition.<br>

-As, our SSIM is ~28.5% we can say that the image user provided is fake or tampered.<br>

-Finally we visualized the differences and similarities between the images using by displaying the images with contours, difference and threshold.<br>

### Novelty :<br/> ###
●	This project can be used in different organizations where customers or users need to provide any kind of id in order to get themselves verified.<br>

● The organization can use this project to find out whether the ID is original or fake. Similarly this can be used for any type of ID like adhar, voter id, etc.<br>

