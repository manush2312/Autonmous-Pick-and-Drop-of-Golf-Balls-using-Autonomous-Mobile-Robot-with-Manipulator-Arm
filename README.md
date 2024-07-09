> [!NOTE]
> Due to company policies, I am unable to share any of the code. However, I can explain the approach we took to achieve this milestone.

# Autonmous-Pick-and-Drop-of-Golf-Balls-using-Autonomous-Mobile-Robot-with-Manipulator-Arm

We are tasked with commanding an Autonomous Mobile Robot (AMR) equipped with a Manipulator Arm to pick up a specific golf ball (either red or blue) and place it into a mug. This involves directing the robot to locate and identify the golf balls using its onboard sensors or vision system. Once identified, the Manipulator Arm will carefully grasp the selected ball and transport it to the designated location of the mug. The robot will then release the ball into the mug, completing the task.

# Flowchart
![Screenshot from 2024-07-09 12-56-55](https://github.com/manush2312/Autonmous-Pick-and-Drop-of-Golf-Balls-using-Autonomous-Mobile-Robot-with-Manipulator-Arm/assets/112979444/852d5eaf-361d-4bcc-8f5a-d594b768ff02)

# Approach
1. Firstly, we need to generate a dataset to train our YOLO model. To achieve this, we manually recorded videos of our two golf balls and the mug. Subsequently, we extracted frames from these videos to obtain photos.
   ```bash
   ffmpeg -i input.mp4 -r 10 frame%04d.png
   The -r 10 argument instructs FFmpeg to extract at a frame rate of 10 fps.



