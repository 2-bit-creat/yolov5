# yolov5

-python3 train.py --img 640 --batch 16 --epochs 5 --data [name].yaml --weights [model_name].pt
$ python3 train.py --img 640 --batch 16 --epochs 5 --data custom_data.yaml --weights yolov5s.pt
- execute
$ python3 detect.py --source 0 --weights best.pt


-custom_data.yaml file is located in yolov5 file
path: ../datasets/custom 
train: images/train  
val: images/valid  

# Classes
nc: 2  # number of classes
names: ['slowly', 'walkroad']  # class names

-file system
yolo
	datasets
		custom
			images
				train
				valid
			labels
				train
				valid
	yolov5
		best.pt
		yolov5s.pt
		custom_data.yaml
			
