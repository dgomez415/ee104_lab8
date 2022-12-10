# Authors: Osman Saeday, David Gomez

# Demonstrations
Link to Image Detection demonstration: https://youtu.be/u0Vpp5sHOaY
Link to Dance Challenge demonstration: https://youtu.be/_9BjQh-1mLM

# References:
1. "YOLOv5 Object Detection on Windows (Step-By-Step Tutorial)": https://wandb.ai/onlineinference/YOLO/reports/YOLOv5-Object-Detection-on-Windows-Step-By-Step-Tutorial---VmlldzoxMDQwNzk4
2. "Collect and Label Images to Train a YOLOv5 Object Detection Model in PyTorch": https://wandb.ai/onlineinference/YOLO/reports/Collect-and-Label-Images-to-Train-a-YOLOv5-Object-Detection-Model-in-PyTorch--VmlldzoxMzQxODc3
3. COCO128 YOLOv5 Dataset - https://github.com/ultralytics/yolov5/releases/download/v1.0/coco128.zip

# YOLOv5 Image Detection

Steps to run the code:
1. Follow the tutorial in Reference 1 to install the appropriate libraries and programs (Python 3.8 or greater, Yolov5 repository, PyTorch, CUDA)
2. In the YOLOv5 folder, enter the command line and enter "python detect.py --source 0 --weights C:\yolov5\runs\train\exp33\weights\best.pt"

The new object added to the YOLOv5 image detection model was "sneaker". In the YAML file "coco128_ee104.yaml", the user can see the complete list of
objects this model is able to detect. Exp33 is the model we had best success with to detect the images through the USB webcam. The parameters used for training
were Epochs = 100, YOLOv5 model = yolov5m, Image resolution = 640. With these parameters, the model was successfully able to recognize our new object "sneaker".
Check video demonstration above to see what the code will do once ran. The file "yolov5" contains a folder called "dataset" which contains
the dataset used for training and a folder called "runs". In runs\train\ there is a folder called "exp33" which contains the demonstrated model used for
detecting the new object "sneaker". 

# Dance Challenge game

The game was the "Dance Challenge" game from the "Coding Games in Python" book. Our goal was to add three tweaks to the code given in the book: Longer Dances,
Play Against a Friend, and Change the Music. All of these tweaks were successfully implemented. Check video above for a demonstration.

Steps to run the code:
1. Make sure pygame and pgzero are installed by typing the following commands into your command prompt:
	pip install pygame
	pip install pgzero
2. Drag "Dance_Challenge.py" into IDE
3. Click run

Additionally: Make sure the images and music folders are in the same directory as the .py

Functionalities Added:
1. Dance length increases by 1 every time both players pass a level
2. Two players, WASD key presses register
3. Music changed 
