# Waste-Classification-Using-Computer-Vision
An automated waste classification system



This code is an implementation of a waste classification system using a pre-trained deep learning model. The system uses a webcam to capture an image of waste material and classifies it into one of four categories - Recyclable, Hazardous, Food, and Residual.

The code starts by importing necessary libraries and modules such as OpenCV, cvzone, and the pre-trained classification model 'Classifier' from the cvzone package. It then initializes the webcam using the 'VideoCapture' function and loads the pre-trained classification model and labels file.

The code then imports the waste and wastebin images from their respective folders using the 'os' and 'cv2' libraries. It also creates a dictionary to map the class IDs to their corresponding wastebin images.

The main loop of the code starts by capturing an image from the webcam and resizing it to a specific size. It then overlays this image on a background image and passes the captured image to the 'getPrediction' function of the 'Classifier' model to get the predicted class ID. If the predicted class ID is not zero, it overlays the corresponding waste image and an arrow image on the background. It also gets the corresponding wastebin image ID from the dictionary and overlays it on the background.

Finally, the code overlays the resized image on the background and displays the output image using the 'imshow' function. The code runs continuously in the loop until the user exits the program using the 'waitKey' function.

This code can be used as a starting point for building a waste classification system using deep learning. However, it would need to be modified and optimized according to the specific use case and environment





Here's what the code does:

1.Import necessary libraries:

   os: used for handling file paths and directories\n
   cvzone: a library that provides various computer vision functions such as object classification, face detection, etc.\n
   cv2: the OpenCV library for image processing.

2.Initialize the video capture object 'cap' with the ID of the camera to be used for capturing images.

3.Load a pre-trained classification model from the specified file path using the 'Classifier' class from CVZone.

4.Load waste images and waste bin images from the specified directories using the 'os' and 'cv2' libraries.

5.Create a dictionary 'classDic' that maps the predicted class ID to the corresponding waste bin ID.

6.In a while loop, read a frame from the video capture object.

7.Resize the captured image to a fixed size.

8.Overlay a background image on the captured image.

9.Use the pre-trained classification model to predict the class of the object in the captured image.

10.If the predicted class is not 0, overlay the corresponding waste image on the background image at a specified position and overlay an arrow image pointing to the waste bin.

11.Use the 'classDic' dictionary to determine the waste bin ID based on the predicted waste class ID.

12.Overlay the corresponding waste bin image on the background image at a specified position.

13.Overlay the resized captured image on the background image at a specified position.

14.Display the resulting image in a window.

15.Wait for a key press event for a specified time.

This code uses the CVZone library's pre-trained model for waste classification and image overlaying functions to create a simple waste classification and disposal application.
