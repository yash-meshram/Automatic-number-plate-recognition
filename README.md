# Automatic-number-plate-recognition.

Project Name: Automatic number plate recognition.

NOTE: All the code written by keeping in mind the application which is mention below. Our test video also depends on our application.\
## ● File descriptions:
  ○ output_plate_image: In this file, all the plate images will be saved\
  ○ indian_license_plate.xml: This is the ".xml" file which will detect the no. plate of the vehicle. We used this file in our code in line 22.\
  ○ liceneplate.xml: This is another ".xml" file which also can be used to detect the no. plate of the vehicle.\
  ○ no._plate_detection.ipynb: This file contains the main code. You can run this file in a jupyter notebook or in the jupyter lab.\
  ○ no._plate_detection.py: This file is just the ".py" file of the above ".ipynb" file. \
  ○ 7.6.2020.xlsx: This is the excel file created by the code. Each day a new ".xlsx" file will be created.
    
    

## ● Videos:
  ○ q2.mp4: This is our testing video. We used this video in our code line 15.\
  ○ Demo.mp4: This video is our code demonstration video.\
  ○ Demo2.mp4: This video is our code demonstration video.
## ● About code:
  ○ Language: Python \
  ○ Libraries used:\
    ■   OpenCV: for image-processing\
    ■   openpyxl: for creating and editing ".xlsx" file\
    ■   pytesseract: for converting text-image to text(string)\
    ■   datetime: for finding the current date and time\
    ■   Os
## ● Short explanation of the code:
  1.   Imported the required packages
  2.   Read the frames of the video
  3.   Detected the number plate of the car by using the “indian_license_plate.xml” file.
  4.   Make a list named “X” and “Y”. In that list, we will add the x and y coordinates of the detected plate.
  5.   When the number of elements reached to 5, we will see whether the (2/3)*(height of full image) is in between the 1st and last elements of the “Y” set or not.
  6.   We had chosen (2/3)*(height of the full image) as an entry line(red line in the video). If the vehicle moves from above red line to below red line then it means that the car had entered IN and vice versa.
  7.   We then save the image of the number plate in file “output_plate_image”.
  8.   After that, we will break the number plate imaged saved, and by using pytesseract we will get the string which is the number on the number plate detected.


NOTE: The process of saving the image and then identifying the text in the image and then adding it in .xlsx file takes time. Therefore you will see that video will stop when the vehicle reaches the read line but after a few seconds, the video will continue. Another thing is that the pytesseract does not convert the image into text fully correctly. There will be some error in image to text. We had tried using mnist dataset but the results were almost the same as that of pytesseract. Therefore we used pytesseract.
## ● APPLICATION:
  ○ To detected and note down the number plate of the vehicle entering the house, official building, shopping mall, college, etc.

NOTE: According to our application and code, we have to use the video in which the camera angle should be in a way that the number plate of the vehicle should be visible clearly. It will be great if we put the camera angle as set in the video “q2.mp4”.

# Youtube link: https://youtu.be/mcqmqyfZ6e8
