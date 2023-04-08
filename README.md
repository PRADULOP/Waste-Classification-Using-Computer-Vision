# Waste-Classification-Using-Computer-Vision
An automated waste classification system



This code is an implementation of a waste classification system using a pre-trained deep learning model. The system uses a webcam to capture an image of waste material and classifies it into one of four categories - Recyclable, Hazardous, Food, and Residual.

The code starts by importing necessary libraries and modules such as OpenCV, cvzone, and the pre-trained classification model 'Classifier' from the cvzone package. It then initializes the webcam using the 'VideoCapture' function and loads the pre-trained classification model and labels file.

The code then imports the waste and wastebin images from their respective folders using the 'os' and 'cv2' libraries. It also creates a dictionary to map the class IDs to their corresponding wastebin images.

The main loop of the code starts by capturing an image from the webcam and resizing it to a specific size. It then overlays this image on a background image and passes the captured image to the 'getPrediction' function of the 'Classifier' model to get the predicted class ID. If the predicted class ID is not zero, it overlays the corresponding waste image and an arrow image on the background. It also gets the corresponding wastebin image ID from the dictionary and overlays it on the background.

Finally, the code overlays the resized image on the background and displays the output image using the 'imshow' function. The code runs continuously in the loop until the user exits the program using the 'waitKey' function.

This code can be used as a starting point for building a waste classification system using deep learning. However, it would need to be modified and optimized according to the specific use case and environment
