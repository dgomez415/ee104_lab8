Authors: Osman Saeday, David Gomez
-----
Link to Image Detection demonstration: https://youtu.be/u0Vpp5sHOaY
Link to Dance Challenge demonstration:
-----
Prior to using code, make sure you have the following installed/downloaded: Python 3.8 or greater, Yolov5 repository, PyTorch, CUDA, OpenLabelling
-----
References:
1. "YOLOv5 Object Detection on Windows (Step-By-Step Tutorial)": https://wandb.ai/onlineinference/YOLO/reports/YOLOv5-Object-Detection-on-Windows-Step-By-Step-Tutorial---VmlldzoxMDQwNzk4
2. "Collect and Label Images to Train a YOLOv5 Object Detection Model in PyTorch": https://wandb.ai/onlineinference/YOLO/reports/Collect-and-Label-Images-to-Train-a-YOLOv5-Object-Detection-Model-in-PyTorch--VmlldzoxMzQxODc3
3. COCO128 YOLOv5 Dataset - https://github.com/ultralytics/yolov5/releases/download/v1.0/coco128.zip
-----
Lab 8 contained two parts: An image detection which involved us adding a new object to detected via a USB webcam and a Simon-says type game where the user's
objective is to follow the dance patterns of the computer.

The new object added to the YOLOv5 image detection model was "sneaker". In the YAML file "coco128_ee104.yaml", the user can see the complete list of
objects this model is able to detect. Exp33 is the model we had best success with to detect the images through the USB webcam. The parameters used for training
were Epochs = 100, YOLOv5 model = yolov5m, Image resolution = 640. With these parameters, the model was successfully able to recognize our new object "sneaker".
Check video demonstration above to see what the code will do once ran. The file "yolov5" contains a folder called "dataset" which contains
the dataset used for training and a folder called "runs". In runs\train\ there is a folder called "exp33" which contains the demonstrated model used for
detecting the new object "sneaker". To run the code yourself, open the command prompt in C:\yolov5, and enter
"python detect.py --source 0 --weights C:\yolov5\runs\train\exp33\weights\best.pt". The git version given only has the best.pt file, but no results due to lack of space allowed on Github.

The game was the "Dance Challenge" game from the "Coding Games in Python" book. Our goal was to add three tweaks to the code given in the book: Longer Dances,
Play Against a Friend, and Change the Music. All of these tweaks were successfully implemented. Check video above for a demonstration.
