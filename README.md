# Barcode-Finding-and-Reading
Mowito Project

Read me: 

The following project is for detecting and decoding barcodes in a given image using Fast R-CNN and Pyzbar library.  Below are the steps

Object detection is performed in the image using Fast R-CNN to get the potential regions. 
Then the potential regions are filtered using  confidence score removing less probable objects and using NMS threshold score to remove overlapping bounding boxes to get the final regions of interest.
The final regions of interest in the image are chosen and image processing techniques such as conversion to grayscale, scaling and thresholding are applied.
The image processed regions of interest are then sent as input to the pyzbar library for decoding barcodes. 

Key Results: 

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

All barcode:

Barcode: 8901719112737 Count: 1
--------------------
Barcode: http://everestspices.com/?ref=qr Count: 1
--------------------
Barcode: 8901030656026 Count: 1
--------------------
Barcode: http://qr.w69b.com/g/ogRXOfCg0 Count: 1
--------------------
Barcode: 8901030574252 Count: 1
--------------------
Total No of barcodes detected:  5

![IMG_20220303_173611](https://github.com/Santoshsrini/Barcode-Finding-and-Reading/assets/28926309/2e26b7b5-4143-4df7-8b8b-6c1c58cb6443)


![IMG_20220303_173846](https://github.com/Santoshsrini/Barcode-Finding-and-Reading/assets/28926309/344847d5-a863-4f4f-8d43-8267ee134197)


![IMG_20220303_175539](https://github.com/Santoshsrini/Barcode-Finding-and-Reading/assets/28926309/00ef08ce-7767-42c3-a5bb-c5894f3b5497)
![IMG_20220303_175324](https://github.com/Santoshsrini/Barcode-Finding-and-Reading/assets/28926309/65b97e46-015d-43be-9428-0ff8a50f7e11)


Missing and Partial Barcode:

IMG_20220303_174744.jpg

![IMG_20220303_174744](https://github.com/Santoshsrini/Barcode-Finding-and-Reading/assets/28926309/e9f6a86f-9a6f-498c-b491-0602bd7b2e57)


Missing Barcodes:


![IMG_20220303_174028](https://github.com/Santoshsrini/Barcode-Finding-and-Reading/assets/28926309/262d4a3b-317e-4aae-9b23-0a173753ce7b)
![IMG_20220303_174953](https://github.com/Santoshsrini/Barcode-Finding-and-Reading/assets/28926309/5724efc0-35c9-4bb1-b153-69e974baf10c)
![IMG_20220303_175557](https://github.com/Santoshsrini/Barcode-Finding-and-Reading/assets/28926309/ec535e17-0b4c-4fd4-ac39-af50b71ad3ba)
![IMG_20220303_175627](https://github.com/Santoshsrini/Barcode-Finding-and-Reading/assets/28926309/b034bd3b-7c12-40a9-9d80-557932271e35)

Partial Barcode:

![IMG_20220303_173853_compressed](https://github.com/Santoshsrini/Barcode-Finding-and-Reading/assets/28926309/5353e3d2-db2d-4c40-92ff-9947fc428e9a)


![IMG_20220303_174238](https://github.com/Santoshsrini/Barcode-Finding-and-Reading/assets/28926309/23703d30-64de-4851-a2f4-17c5d2515c56)
![IMG_20220303_175317](https://github.com/Santoshsrini/Barcode-Finding-and-Reading/assets/28926309/dfcf1a90-3611-4238-aa5e-f860dd66dab7)
![IMG_20220303_175451](https://github.com/Santoshsrini/Barcode-Finding-and-Reading/assets/28926309/bc56ba71-1d10-4197-9307-ca4484b822ab)




