# Real-Time-Human-Detection
> Real-time human detection is an important application of computer vision that involves identifying human figures within an image, video or live camera feed. The real-time human detection script provided here uses OpenCV and HOG descriptors to detect and draw a box around human figures in a given input.

> The script provides three ways to detect humans: through an image, video or live camera feed. If an image is used as input, the script detects human figures and draws a box around them, saving the output as a new image. If a video file is used, the script reads each frame and applies the same detection algorithm, saving the output as a new video file if an output path is specified. If a live camera feed is used, the script continuously reads the camera input and applies the detection algorithm to the video feed in real-time.

> The human detection algorithm used in the script is based on HOG descriptors, which are machine learning features that help to identify human figures. The script sets up the HOG descriptor object and specifies the default people detector using the setSVMDetector() function. The detectMultiScale() function is then used to apply the HOG descriptor object to the input image or video frame to detect the human figures.

> The script also uses the imutils library to resize the input image or video frame to ensure that it is of manageable size. It then draws a green box around each detected human figure and labels them with a number. The script also displays the number of human figures detected in the input, updating this number in real-time as the detection algorithm runs.

> Overall, the real-time human detection script provides a simple and effective way to detect human figures in a range of scenarios using computer vision techniques. This has a wide range of practical applications, including security, surveillance, and video analysis in industries such as healthcare and retail.

## REQUIREMENTS:
Write this in terminal to install these libraries:
```
pip install opencv-python
```
```
pip install imutils
```

- **For Video:** Type this code in terminal with the video address
```python
python rthd.py -v "[video file]"
```

## INPUTS:
- **For Image:** Type this code in terminal with the image address
```python
python rthd.py -i "[image file]"
```

- **For Video:** Type this code in terminal with the video address
```python
python rthd.py -v "[video file]"
```

- **For Camera(Webcam):** Type this code in terminal
```python
python rthd.py -c true
```

## OUTPUT:
### - **Image**
![image](https://user-images.githubusercontent.com/70787869/229260827-e5975889-42ef-4263-9e22-fbfc75aeaf86.png)

### - **Video**
![image](https://user-images.githubusercontent.com/70787869/229261091-0e066688-daeb-4e07-aba7-6afcc4e80dc1.png)

### - **Webcam**
![image](https://user-images.githubusercontent.com/70787869/229261186-387f4c6b-1ba9-46bd-a6ab-82e58a67012e.png)


#### Note: To quit the running process - press "q"
Thank you and Enjoy Data Science 'n' Coding 😉
