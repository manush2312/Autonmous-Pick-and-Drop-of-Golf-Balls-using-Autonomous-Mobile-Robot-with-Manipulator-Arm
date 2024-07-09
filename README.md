> [!NOTE]
> Due to company policies, I am unable to share any of the code. However, I can explain the approach we took to achieve this milestone.

> [!TIP]
> We have primarily utilized NVIDIA platforms for this project.

# Autonmous-Pick-and-Drop-of-Golf-Balls-using-Autonomous-Mobile-Robot-with-Manipulator-Arm

We are tasked with commanding an Autonomous Mobile Robot (AMR) equipped with a Manipulator Arm to pick up a specific golf ball (either red or blue) and place it into a mug. This involves directing the robot to locate and identify the golf balls using its onboard sensors or vision system. Once identified, the Manipulator Arm will carefully grasp the selected ball and transport it to the designated location of the mug. The robot will then release the ball into the mug, completing the task.

# Flowchart
![Screenshot from 2024-07-09 14-31-23](https://github.com/manush2312/Autonmous-Pick-and-Drop-of-Golf-Balls-using-Autonomous-Mobile-Robot-with-Manipulator-Arm/assets/112979444/36c5b6d7-ede7-420c-a54d-7b66a0f80ee7)

# Approach
1. Firstly, we will give a voice command indicating which ball to pick, which will be recorded into a WAV file.
2. The recorded WAV file will be passed to the NVIDIA RIVA API, which converts speech to text.
3. The extracted text file will be passed to an LSTM model, which will provide us with the class ID of the required ball.
4. The obtained class ID will be passed to the YOLO model, which performs the object detection task.
5. Now our Autonomous Mobile Robot will track the object, in our case ball, and will navigate towards it.
6. Our AMR will reach the required ball and pick it up using its manipulator arm.
7. Now, it will detect the mug and move towards it.
8. On reaching the mug, it will drop the ball.

# Links
The link for the results and dataset preparation is (Link)[https://drive.google.com/drive/folders/1n4rmUuMtyVJSERog5-JxNLMLBKBPAsAK?usp=sharing].
