# ADAS USING DROWSINESS DETECTION

**Intro:**
<br>
Through the means of a cabin mounted camera, powered with computer vision and machine learning algorithms, we can monitor the driver’s status.
The driver drowsiness detection algorithm begins recording the driver’s visual eyelid behavior the moment the trip begins.
It then recognizes changes over the course of the trip, and thus also the driver’s state of fatigue.


**Methodology:**
<br>
The project is based on behavioral measures. In behavioral measuring or visual based approach different gestures of 
the driver like eye blink are monitored to examine the state of the driver. The following steps are considered to monitor the driver.

- The algorithm detects the face in the pre-processed image by using facial landmarks produced by Dlib library.
- In the detected face region, the algorithm finds the face landmark.
- To detect eye region, the correct array slices from the set of face landmarks is detected.
- Calculate EAR (eye aspect ratio) to determine whether the eyes of the driver are closed or not while driving.
- Check to see if the eye aspect ratio is below the “blink/closed” eye threshold.
- If it is, increment DROWSY, the total number of consecutive frames where the person has had their eyes closed.


