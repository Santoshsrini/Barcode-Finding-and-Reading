# Barcode-Finding-and-Reading
Mowito Project

The following project is for detecting and decoding barcodes in a given image using Fast R-CNN and Pyzbar library.  Below are the steps

Object detection is performed in the image using Fast R-CNN to get the potential regions. 
Then the potential regions are filtered using  confidence score removing less probable objects and using NMS threshold score to remove overlapping bounding boxes to get the final regions of interest.
The final regions of interest in the image are chosen and image processing techniques such as conversion to grayscale, scaling and thresholding are applied.
The image processed regions of interest are then sent as input to the pyzbar library for decoding barcodes. 

## Key Results: 

Barcode values along with the number of appearances in the image are printed.
Bounding box of black color is displayed around every object that has a barcode. 
Bounding box of blue color and the barcode value is displayed around the barcode detected. 
Bounding box of red is displayed around the object that doesn't have a barcode. 

Resulting images after performing the algorithm are saved in the folders - all barcodes, partial and missing barcodes, missing barcodes, partial barcodes. 

How to run the code: 

Save the images by creating Mowito Project/sample/ type of barcode/ image no: Example:

My Drive/Mowtio Project/sample/partial barcode/IMG_20220303_175451.jpg')

All necessary packages can be imported during execution. 

Run all cells to execute. 


Key Results:

## All barcode:

![IMG_20220303_173611](https://github.com/Santoshsrini/Barcode-Finding-and-Reading/assets/28926309/2e26b7b5-4143-4df7-8b8b-6c1c58cb6443)

Barcodes: 8901719112737 Count: 1

Barcode: http://everestspices.com/?ref=qr Count: 1

Barcode: 8901030656026 Count: 1

Barcode: http://qr.w69b.com/g/ogRXOfCg0 Count: 1

Barcode: 8901030574252 Count: 1

<br/>
<br/>

![IMG_20220303_173846](https://github.com/Santoshsrini/Barcode-Finding-and-Reading/assets/28926309/344847d5-a863-4f4f-8d43-8267ee134197)

Barcode: 8901030578199 Count: 1

Barcode: 8901030609350 Count: 1

Barcode: 8901030781063 Count: 1

Barcode: 8901063160088 Count: 1

Barcode: 8901030656026 Count: 1

Barcode: http://everestspices.com/?ref=qr Count: 2

Barcode: 8901725114916 Count: 3

Barcode: 8906021125000 Count: 1

Total No of barcodes detected:  11

<br/>
<br/>

![IMG_20220303_175539](https://github.com/Santoshsrini/Barcode-Finding-and-Reading/assets/28926309/00ef08ce-7767-42c3-a5bb-c5894f3b5497)

Total No of barcodes detected:  0

<br/>
<br/>


![IMG_20220303_175324](https://github.com/Santoshsrini/Barcode-Finding-and-Reading/assets/28926309/65b97e46-015d-43be-9428-0ff8a50f7e11)

Barcode: 8901719110856 Count: 1

Total No of barcodes detected:  1

<br/>
<br/>


## Missing and Partial Barcode:

![IMG_20220303_174744](https://github.com/Santoshsrini/Barcode-Finding-and-Reading/assets/28926309/e9f6a86f-9a6f-498c-b491-0602bd7b2e57)

Barcode: 8901030795589 Count: 1

Barcode: 8901725118457 Count: 1

Total No of barcodes detected:  2


<br/>
<br/>

## Missing Barcodes:

![IMG_20220303_174028](https://github.com/Santoshsrini/Barcode-Finding-and-Reading/assets/28926309/262d4a3b-317e-4aae-9b23-0a173753ce7b)

Barcode: http://qr.w69b.com/g/ogRXOfCg0 Count: 1

Barcode: 8901030656026 Count: 2

Barcode: 8901030578199 Count: 1

Barcode: http://everestspices.com/?ref=qr Count: 2

Barcode: 8901030112737 Count: 1

Barcode: 8901030781063 Count: 1

Barcode: 8901030609350 Count: 2

Total No of barcodes detected:  10

<br/>
<br/>

![IMG_20220303_174953](https://github.com/Santoshsrini/Barcode-Finding-and-Reading/assets/28926309/5724efc0-35c9-4bb1-b153-69e974baf10c)

Barcode: 8901725118457 Count: 1

Total No of barcodes detected:  1

<br/>
<br/>

![IMG_20220303_175557](https://github.com/Santoshsrini/Barcode-Finding-and-Reading/assets/28926309/ec535e17-0b4c-4fd4-ac39-af50b71ad3ba)

Total No of barcodes detected:  0

<br/>
<br/>

![IMG_20220303_175627](https://github.com/Santoshsrini/Barcode-Finding-and-Reading/assets/28926309/b034bd3b-7c12-40a9-9d80-557932271e35)


Total No of barcodes detected:  0

<br/>
<br/>


## Partial Barcode:

![IMG_20220303_173853_compressed](https://github.com/Santoshsrini/Barcode-Finding-and-Reading/assets/28926309/5353e3d2-db2d-4c40-92ff-9947fc428e9a)

Barcode: 8901063160088 Count: 2

Barcode: 8901030656026 Count: 1

Barcode: http://everestspices.com/?ref=qr Count: 2

Barcode: 8901030609350 Count: 1

Barcode: 8901725114916 Count: 2

Total No of barcodes detected:  8

<br/>
<br/>

![IMG_20220303_174238](https://github.com/Santoshsrini/Barcode-Finding-and-Reading/assets/28926309/23703d30-64de-4851-a2f4-17c5d2515c56)

Total No of barcodes detected:  0

<br/>
<br/>

![IMG_20220303_175317](https://github.com/Santoshsrini/Barcode-Finding-and-Reading/assets/28926309/dfcf1a90-3611-4238-aa5e-f860dd66dab7)

Barcode: 8901719110856 Count: 2

Total No of barcodes detected:  2

<br/>
<br/>

![IMG_20220303_175451](https://github.com/Santoshsrini/Barcode-Finding-and-Reading/assets/28926309/bc56ba71-1d10-4197-9307-ca4484b822ab)

Total No of barcodes detected:  0

<br/>
<br/>

# Lead-up methods:

## Only using the Pyzbar Library: 

Only using the pyzbar library for barcode detection didn't give the best accuracy. Pyzbar works better when a small region is given as input. Accuracy was better when the detected object was passed for barcode detection. 

![download (1)_compressed](https://github.com/Santoshsrini/Barcode-Finding-and-Reading/assets/28926309/18ac50f6-ca20-469a-9220-fcd29faf340c)


## Using Contour detection techniques:

![contour_compressed](https://github.com/Santoshsrini/Barcode-Finding-and-Reading/assets/28926309/92e6a240-2300-49e4-8fc0-1e392bbb097c)


Tried performing object detection using contour detection. But detected regions were too many than the actual number.


![cluster contours_compressed](https://github.com/Santoshsrini/Barcode-Finding-and-Reading/assets/28926309/a3fbefdb-1d5d-4219-a65c-49dd48ad6851)

Tried combining several contours by concatening them based on clusters. But the issue here was how do you predetermine the number of clusters. There were methods where the algorithm itself could compute the optimal number but even these required a maximum number. Above was for 4 clusters.

Performed several other contour detection techniques too such as aplying gradients, performing image processing such as dilation before contour detection but once again accuracy was poor. 

![image](https://github.com/Santoshsrini/Barcode-Finding-and-Reading/assets/28926309/69e9e84d-5646-43fb-ae65-b289cb1ac04d)


** Came to conclusion that for object detection ML models were the best option **

## Using YOLO:

Tried YOLO but none of the objects were detected as they were not part of training labels, so didn't use this. But in the future, maybe thought of using transfer learning by adding a new label called as "unknown" and then predicting. 

## Using Fast-R CNN:

Fast R-CNN gave results in predicting the object detection regions although the label it predicted was for " books " but nonetheless it served the purpose as the region mattered more than the prediction. 

![object detection using fast r cnn_compressed](https://github.com/Santoshsrini/Barcode-Finding-and-Reading/assets/28926309/778ec08e-6077-4eb1-b659-e772ee17df0d)

But this gave many overlapping bounding boxes, so performed NMS to reduce the overlap. 

![nms obj detection_compressed](https://github.com/Santoshsrini/Barcode-Finding-and-Reading/assets/28926309/581bd566-ebf9-4c21-b57c-95c0f955297f)


Then performed barcode detection passing each finally obtained region for pyzbar. Before passing scaling, grayscale conversion and thresholding were applied. The parameters for each of these were set based on experimentation ( eg: scaling to 4x gave a better accuarcy instead of 2x etc. )
