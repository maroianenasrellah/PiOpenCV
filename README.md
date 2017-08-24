# PiOpenCV
Instruction to install OpenCV on Raspberry Pi

Based on the 
[Install guide: Raspberry Pi 3 + Raspbian Jessie + OpenCV 3.](http://www.pyimagesearch.com/2016/04/18/install-guide-raspberry-pi-3-raspbian-jessie-opencv-3/) from pyimagesearch.com


# Steps

## Step #1: Expand filesystem
```bash
sudo apt-get purge wolfram-engine
```

## Step #2: Install dependencies
```bash
sudo apt-get install build-essential cmake pkg-config

sudo apt-get install libjpeg-dev libtiff5-dev libjasper-dev libpng12-dev
sudo apt-get install libavcodec-dev libavformat-dev libswscale-dev libv4l-dev
sudo apt-get install libxvidcore-dev libx264-dev
sudo apt-get install libgtk2.0-dev
sudo apt-get install libatlas-base-dev gfortran

sudo apt-get install python3-dev
```

## Step #3: Download the OpenCV source code
```bash
cd ~
mkdir src
cd src
wget -O opencv.zip https://github.com/opencv/opencv/archive/3.3.0.zip
unzip opencv.zip
```

Optionally, install contrib package.
```bash
wget -O opencv_contrib.zip https://github.com/opencv/opencv_contrib/archive/3.3.0.zip
unzip opencv_contrib.zip
```


## Step #4: Python 2.7 or Python 3?
