# FACIAL SURVEILLANCE USING RASPBERRYPI AND C++
This is a facial-recognition and authentication project using raspberry pi 
This C++ application recognizes a person from a database of more than 2000 faces.  It is built for a Raspberry PI 4, but can easily be ported to other platforms.

First, the faces and their landmarks are detected by **RetinaFace** or **MTCNN**.
Next, the database is scanned with **Arcface** for the matching face.
In the end, **Face Anti Spoofing** tests whether the person in front of the camera is real and not a mask or a cardboard photo.

If the face is not found in the database, it will be **added automatically**. A **blur** filter ensures only sharp faces in the database. One photo per person is sufficient, although more does not hurt.

## DEPENDENCIES
To run the application, you have to:
- A raspberry Pi 4 with a 64-bit operating system. It can be the Raspberry 64-bit OS, or Ubuntu 18.04 / 20.04. [Install 64-bit OS](https://qengineering.eu/install-raspberry-64-os.html) <br/>
- The Tencent ncnn framework installed. [Install ncnn](https://qengineering.eu/install-ncnn-on-raspberry-pi-4.html) <br/>
- OpenCV 64 bit installed. [Install OpenCV 4.5](https://qengineering.eu/install-opencv-4.5-on-raspberry-64-os.html) <br/>
- Code::Blocks installed. (`$ sudo apt-get install codeblocks`)

## REFERENCES
* https://github.com/Qengineering/Face-Recognition-Raspberry-Pi-64-bits
