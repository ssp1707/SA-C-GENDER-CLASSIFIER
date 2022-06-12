# <p align="center"> SA-C-GENDER-CLASSIFIER </p>
# Algorithm
1. Install the DeepFace library using the command pip install deepface
2. To Predict the gender of a person use this DeepFace library
3. Import the deepface class from DeepFace library, cv2 class from openCv2 library and Matplot library according to the requirements.
4. Load and display the image which we have imported. 
5. Pass the image to DeepFace library and analyze the image to predict gender of a person.
6. This prediction is stored in result variable and print the prediction using this algorithm.

## Program:
```

Developed by   : S. Sanjna Priya
RegisterNumber :  212220230043

```

```
!pip install deepface
from deepface import DeepFace
import cv2
import matplotlib.pyplot as plt
img1=cv2.imread('ts.jpg')
plt.imshow(img1[:,:,::-1])
plt.show()
result=DeepFace.analyze(img1,actions=['gender'])
print("Gender : ",result['gender'])
img2=cv2.imread('vj.jpg')
plt.imshow(img1[:,:,::-1])
plt.show()
result=DeepFace.analyze(img2,actions=['gender'])
print("Gender : ",result['gender'])
```

## OUTPUT:

![SA 1](https://user-images.githubusercontent.com/75234965/173235757-655c858b-00a1-4097-9214-b2c28832828a.PNG)

![SA 2](https://user-images.githubusercontent.com/75234965/173235764-a5fd707b-c278-4b8b-8d8f-962eba7b3ce8.PNG)

DEMO VIDEO YOUTUBE LINK:

https://youtu.be/yhzBbxh-SyE
