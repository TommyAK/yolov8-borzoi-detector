
# YOLOv8 Borzoi Detector

Training a YOLOv8 model from Ultralytics on a custom dataset consisting of borzoi dogs extracted from various sources across the internet for recognition and detection. 

<img src="https://github.com/TommyAK/yolov8-borzoi-detector/assets/35144580/0c38d206-c985-4819-8458-c48896938f96" width=60% height=60%>
<img src="https://github.com/TommyAK/yolov8-borzoi-detector/assets/35144580/b8c51a4c-3dd9-48dc-b353-ac03a9fa084b" width=60% height=60%>



## Information
I annotated the images using Label Studio [[1]](#1). A bounding box was placed around each borzoi dog that appeared in an image. 

Two python scripts ``yaml_data_file_creator.ipynb`` and ``dataset_splitter.ipynb`` were created to help structure the image files into training, testing, and validation. The export from Label Studio was in a format that was difficult to work with YOLOv8, so these two files ensure proper directory formatting and that a ``data.yaml`` file is created.

Model performed well on videos in addition to photos. Very interesting to see first-hand just how effective neural nets are for image classification and detection and how YOLO can be tailored for a range of applications.


## Prerequisites

- ultralytics
- opencv
- sklearn

## References
<a id="1">[1]</a>
Tkachenko, Maxim, Malyuk, Mikhail, Holmanyuk, Andrey, & Liubimov, Nikolai. (2020). Label Studio: Data labeling software. Retrieved from https://github.com/heartexlabs/label-studio
