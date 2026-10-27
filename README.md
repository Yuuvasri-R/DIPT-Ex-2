
# Image Capture and Video Processing Using OpenCV

# Aim
To write a Python program using OpenCV to capture an image from the webcam and perform the following operations:

Write the frame as a JPG file
Display the video
Display the video by resizing the window
Rotate and display the video
🛠️ Software Used
Anaconda – Python 3.7
Jupyter Notebook / VS Code
OpenCV (cv2)
⚙️ Algorithm
Step 1:
Import the required libraries and initialize the webcam using cv2.VideoCapture().

Step 2:
Capture frames continuously from the webcam.

Step 3:
Save a frame as a JPG image using cv2.imwrite().

Step 4:
Display the live video stream using cv2.imshow().

Step 5:
Resize the frame and rotate it using OpenCV functions, then display the processed frames.

💻 Program
Developed By:
Name: Yuuvasri R

Register No:
212225230313
```
import cv2
import matplotlib.pyplot as plt
from IPython.display import clear_output
import time
cap = cv2.VideoCapture(0)
ret, frame = cap.read()
if ret:
    cv2.imwrite("photo.png", frame)
cap.release()
captured_image = cv2.imread('photo.png')
plt.imshow(captured_image[:,:,::-1])
plt.title('Captured Frame')
plt.axis('off')
plt.show()
cap = cv2.VideoCapture(0)

for i in range(50):
    ret, frame = cap.read()
    if not ret:
        break
    frame_rgb = cv2.cvtColor(frame, cv2.COLOR_BGR2RGB)
    clear_output(wait=True)
    plt.imshow(frame_rgb)
    plt.axis('off')
    plt.show()
    time.sleep(0.05)

cap.release()

cap = cv2.VideoCapture(0)

for i in range(50):
    ret, frame = cap.read()
    if not ret:
        break
    resized_frame = cv2.resize(frame, (100, 150))  # Resize to 320x240
    frame_rgb = cv2.cvtcap = cv2.VideoCapture(0)

for i in range(50):
    ret, frame = cap.read()
    if not ret:
        break
    rotated_frame = cv2.rotate(frame, cv2.ROTATE_90_CLOCKWISE)
    frame_rgb = cv2.cvtColor(rotated_frame, cv2.COLOR_BGR2RGB)
    clear_output(wait=True)
    plt.imshow(frame_rgb)
    plt.axis('off')
    plt.show()
    time.sleep(0.05)
cap.release()
Color(resized_frame, cv2.COLOR_BGR2RGB)
    clear_output(wait=True)
    plt.imshow(frame_rgb)
    plt.axis('off')
    plt.show()
    time.sleep(0.05)
cap.release()
```
# Output
i) Write the frame as JPG image
<img width="580" height="453" alt="image" src="https://github.com/user-attachments/assets/6ab71299-fd9c-4e42-b4e8-802aa2d06743" />

ii) Display the video
<img width="568" height="437" alt="image" src="https://github.com/user-attachments/assets/81c844ba-8204-4fe6-9741-948520ae8475" />

iii) Display the video by resizing the window
<img width="287" height="416" alt="image" src="https://github.com/user-attachments/assets/66f8186a-3edc-43c6-ac76-32119d4e6dd8" />

iv) Rotate and display the video
<img width="311" height="422" alt="image" src="https://github.com/user-attachments/assets/9e9baf75-5820-4cef-b5e3-c39f07f47752" />

# Result
Thus, the image is successfully captured from the webcam and various video processing operations such as saving, displaying, resizing, and rotating are performed using OpenCV.

































































.


















































































































































.














































































































































































































































































.










































.

























































.






















































.










































































































































































.
