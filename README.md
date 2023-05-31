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


Key Results:![IMG_20220303_173611](https://github.com/Santoshsrini/Barcode-Finding-and-Reading/assets/28926309/2e26b7b5-4143-4df7-8b8b-6c1c58cb6443)
![IMG_20220303_173846](https://github.com/Santoshsrini/Barcode-Finding-and-Reading/assets/28926309/344847d5-a863-4f4f-8d43-8267ee134197)


![IMG_20220303_175539](https://github.com/Santoshsrini/Barcode-Finding-and-Reading/assets/28926309/00ef08ce-7767-42c3-a5bb-c5894f3b5497)
![IMG_20220303_175324](https://github.com/Santoshsrini/Barcode-Finding-and-Reading/assets/28926309/65b97e46-015d-43be-9428-0ff8a50f7e11)

