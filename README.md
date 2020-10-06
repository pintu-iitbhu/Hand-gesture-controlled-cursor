# Hand-gesture-controlled-cursor
      
Hand gesture controlled mouse cursor with webcam.

This approach for hand gesture recognition is vision based,which
uses image processing techniques and inputs from a computer webcam.
The input frame captured from webcam is processwed in three part-

--skin detection(using histogram model)

--hand gesture detection(using contour extraction,convex hull detection) 

--Integrating mouse function(using Pyautogui library)

# Our algorithm works as follows:

      Webcam video is captures using c# video capture libraries
      It is broken up into continuous image frames
      Each frame is converted to grayscale
      Each frame is now scanned to check five finger design pattern
      Once detected it is flagged as an object
      System now tracks its movement within particular frame
      This is tracked in terms of x,y coordinates
      These x, coordinates are now mapped onto mouse cursor positioning
