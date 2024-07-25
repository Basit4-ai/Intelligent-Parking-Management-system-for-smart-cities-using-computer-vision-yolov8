# Intelligent-Parking-Management-system-for-smart-cities-using-computer-vision-yolov8
# 1. Project overview
The Intelligent Parking Management System leverages computer vision and YOLOv8 to monitor parking areas in real-time. It detects and classifies parking slots as occupied, available, correctly parked, and wrongly parked. This system aims to streamline parking management, reduce traffic congestion, and enhance urban mobility
#Features
Real-time Detection: Monitors parking slots in real-time.
Slot Classification: Identifies and classifies each slot as occupied, available, right parked, or wrongly parked.
High Accuracy: Utilizes YOLOv8 for precise object detection and classification.
Scalability: Can be scaled for different parking lot sizes and configurations.
# Steps involved for completion of this project
# 1. Data collection:
first a of all we have a design a small prototype of a paking.
we have taken images of this parking slot with different angles 
# 2.Data Preparation using Roboflow
then we have annotate the images as "Car", "Right_parked" and "wrong_parked".
# 3.Model Training:
after annotataion we have trained Yolov8 model on that annotated images and got our model named as 'wrong_car.pt'
this wrong_car.pt model will detect car ,wrog_parked and Right_parked.
# Selecting coordinates :
WE have captured a pic from camera named as "parking_lot.png" and select the coordinates using the file "select slot coordinates.ipynb" and got the final
coordinates as "Final_coodinates.txt"
# Making a logic using OpenCV for the occupancy of parking slot:
we have target  the center of the car as our decision making feature , if the car center enter into the coordinate it will occupied the slot and increment the occopied by one while 
decrement the availabe slot .
# Running the "Final.ipynb" file:
after running the the above file this will detect real time the available slot ,occupied slot ,right_parked and Wrong_parket
