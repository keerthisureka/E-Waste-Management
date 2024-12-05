## Commands to run this project in google colab

### To set up yolov5 environment
```
!git clone https://github.com/ultralytics/yolov5.git
%cd yolov5/
!pip install -qr requirements.txt comet_ml
```

### The files to be copied from this repository into your yolov5 directory
- benchmarks.py
- detect.py
- export.py
- train.py

### Train the model using you dataset
##### Dataset structure (The path is given with refernce to google colab)
```
/content/drive/MyDrive/Dataset/
  ├── images/
  │    ├── train/
  │    │   ├── img1.jpg
  │    │   ├── img2.jpg
  │    │   ├── img3.jpg
  │    ├── val/
  │    │   ├── img4.jpg
  │    │   ├── img5.jpg
  ├── labels/
  │    ├── train/
  │    │   ├── img1.txt
  │    │   ├── img2.txt
  │    ├── val/
  │    │   ├── img4.txt
  │    │   ├── img5.txt
  └── data.yaml
```
- Dataset should be split into 80:20 ratio for train:val.
- Dataset can be downloaded from [Roboflow](https://universe.roboflow.com/) in Yolov5 PyTorch format.

