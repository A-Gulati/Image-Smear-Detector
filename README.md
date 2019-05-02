# Image-Smear-Detector

Objective: Given a folder of images, to detect physical smears on the camera lenses and to generate a mask of these areas.

# Approach to the problem: 

### Pre-process
- Convert to grayscale
- Equalize histogram
- Apply gaussian blur
- Create mean image
### Initial Mask Generation
- Apply adaptive threshold
- Erode
- Dilate
### Find Contours
- Convert image back to rgb (remains black and white)
- Use cv2.findContours to find all contours in image
- Draw contours on to intermediate result and save


