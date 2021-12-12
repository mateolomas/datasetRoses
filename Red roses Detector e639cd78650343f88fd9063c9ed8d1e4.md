# Red roses Detector

## Introduction

---

This software, which is an AI system, will be made with the objective of counting and detecting a type of roses that are in a given image. In order to do this, TensorFlow Lite is be used, where files corresponding to the weights and architecture of the model will be exported. Then, it will be used by other systems, specifically by a web platform and a mobile application.

## Pre-requisites

### Training

---

Install dependencies

```bash
!pip install -q --use-deprecated=legacy-resolver tflite-model-maker
!pip install opencv-python
!pip install pillow
!pip install tensorflow==2.7.0
!pip install numpy==1.21.4
!pip install matplotlib

```

### Testing (Inference)

In order to test our model, you must have install the following dependencies before use the model.

- Python3
- Matplotlib
- Tensorflow=2.7.0
- Numpy=1.21.4
- Pillow
- OpenCV
- Argparse

### Installation

---

1. Clone this repository 

```bash
git clone https://github.com/
cd AI_based 
```

1. Install dependencies

```bash
pip3 install -r requirements.txt 
```

1. You can download a custom Red Rose Image from any of your preferred sources.

## Usage for inference

First, we can use the following command if we need some help

```bash
python3 inference.py --help
```

![Screen Shot 2021-12-11 at 23.36.04.png](Red%20roses%20Detector%20e639cd78650343f88fd9063c9ed8d1e4/Screen_Shot_2021-12-11_at_23.36.04.png)

Then, we are trying with an image called "rose1.jpg". We must use the flag **—image** in order to load an image in the current directory. 

```bash
python3 inference.py --image="rose1.jpg" 
```

We can use the flag **—threshold,** if we want to adjust the threshold parameter. A threshold of 0.5 is set by default. We're trying with 0.4

```bash
python3 inference.py --image="rose1.jpg" --threshold=0.4
```