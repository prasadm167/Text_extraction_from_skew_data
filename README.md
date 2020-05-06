# Text_extraction_from_skew_data
Image have a rotated block of text at an unknown angle so we need to correct it by Detecting the block, compute the angle of text in image
Rotate text in image to correct the skew
we are using cv2.minAreaRect which then computes the  rotated rectangle that contains  text region.
cv2.minAreaRect  function returns angle values in the range [-90, 0).
we will find the center (x,y) coordinates then pass center to cv2.getRotationMatrix2D, post it will display with the angle with 'image2' variable in code
By using pytesseract, we can extract the data from 'image2' variable
