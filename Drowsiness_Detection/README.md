# Drowsiness Detection

If their eyes have been closed for a certain amount of time, we’ll assume that they are starting to doze off and play an alarm to wake them up and grab their attention.

## General Flow

- A camera monitors a stream for faces.
- If a face is found, we apply facial landmark detection and extract the eye regions.
- Now that we have the eye regions, we can compute the eye aspect ratio to determine if the eyes are closed.
- If the eye aspect ratio indicates that the eyes have been closed for a sufficiently long enough amount of time, we’ll sound an alarm to wake up the driver.

### Running the program
Our drowsiness detector requires one command line argument followed by two optional ones, each of which is detailed below:

1) --shape-predictor : This is the path to dlib’s pre-trained facial landmark detector. 
2) --alarm : Here you can optionally specify the path to an input audio file to be used as an alarm.
3) --webcam : This integer controls the index of your built-in webcam/USB camera.

Now run the code by:
	pythob detect_drowsiness.py\
	--shape-predictor shape_predictor_68_face_landmarks.dat\
	--alarm alarm.wav