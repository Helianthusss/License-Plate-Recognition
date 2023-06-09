# License-Plate-Recognition-YOLOv5

This repository provides you with a detailed guide on how to training and build a Vietnamese License Plate detection and recognition system. This system can work on 2 types of license plate in Vietnam, 1 line plates and 2 lines plates.

## Installation

```bash
  https://github.com/Helianthusss/License-Plate-Recognition.git
  cd License-Plate-Recognition

  # install dependencies using pip 
  pip install -r ./requirement.txt
```

- **Pretrained model** provided in ./model folder in this repo 

- **Download yolov5 (old version) from this link:** [yolov5 - google drive](https://drive.google.com/drive/folders/1uCPQAQJaPIQBbjMWKsFDL7UnWXzXar85?usp=share_link)

- Copy yolov5 folder to project folder

## Run License Plate Recognition

```bash
  # run inference on webcam (15-20fps if there is 1 license plate in scene)
  python webcam.py 

  # run inference on image
  python lp_image.py -i test_image/3.jpg

  # run LP_recognition.ipynb if you want to know how model work in each step
```

## Result

#### Image  demo
![Demo](License-Plate-Recognition/result/image.jpg)

#### Video demo
![Video](License-Plate-Recognition/result/video_1.gif)


## Dataset:

- [License Plate Detection Dataset](https://drive.google.com/file/d/1xchPXf7a1r466ngow_W_9bittRqQEf_T/view?usp=sharing)
- [Character Detection Dataset](https://drive.google.com/file/d/1bPux9J0e1mz-_Jssx4XX1-wPGamaS8mI/view?usp=sharing)


## Training

**Training code for Yolov5:**

Use code in ./training folder
```bash
  training/Plate_detection.ipynb     #for LP_Detection
  training/Letter_detection.ipynb    #for Letter_detection
```
