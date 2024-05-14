# OPENING--AND-CLOSING
## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
<br>
Import the necessary packages



### Step2:
<br>
Create the Text using cv2.putText


### Step3:
<br>
Create the structuring element


### Step4:
<br>
Use Opening operation


### Step5:
<br>
Use Closing Operation


 
## Program:

# Import the necessary packages
```
import io
import os
import cv2
import numpy as np
import matplotlib.pyplot as plt
```
# Create the Text using cv2.putText
```
img = np.zeros((100, 400), dtype='uint8')
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img, 'REVERIE !', (5, 70), font, 2, (255), 5, cv2.LINE_AA)

```


# Create the structuring element
```
kernel = np.ones((7, 7), np.uint8)
```


# Use Opening operation
```

image1=cv2.morphologyEx(img1,cv2.MORPH_OPEN,kernel)
plt.imshow(image1)
plt.axis("off")
```



# Use Closing Operation
```



image2=cv2.morphologyEx(img1,cv2.MORPH_CLOSE,kernel)
plt.imshow(image2)
plt.axis("off")




```
## Output:

### Display the input Image

![Screenshot 2024-04-29 221103](https://github.com/Aravindsamy04/OPENING--AND-CLOSING/assets/113497037/00eff406-9eb1-4c35-a637-5c1586f2faf5)


### Display the result of Opening
![Screenshot 2024-04-29 221112](https://github.com/Aravindsamy04/OPENING--AND-CLOSING/assets/113497037/b7cab076-468c-4463-94bb-4e9df1253fc3)


### Display the result of Closing


![Screenshot 2024-04-29 221121](https://github.com/Aravindsamy04/OPENING--AND-CLOSING/assets/113497037/aacae1d1-a4f1-4987-b9b6-28d406aebdf4)


## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
