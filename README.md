# OpenCV-example

This is a simple Python application based on OpenCV library intended to recognize faces of people in the picture.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. 
See deployment for notes on how to deploy the project on a live system.

### Prerequisites

Install all required modules and versions running Dockerfile:

```
docker build -t opencv .
docker run -v  $PWD/code:/home/code  -it opencv bash
```

### Installing

In order to run the script, scripts name should be folloved by 2 parameters: picture name and an XML file that contains the data to detect faces:

```
$ python face_detect.py sample_pictures/picture_name.jpg haarcascade_frontalface_default.xml
```

As a result in console should be written how many faces were recognized. If to many\little, parameters in faces function could be changed.