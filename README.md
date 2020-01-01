# CELLULAR IMAGE CLASSIFICATION


The below project is our solution for the multi-class cellular image classification problem. There were 14 classes of cell images, with a training data of 10,000 images and a test data of 15,000 images.

The key challenges of the problem statement:
--------------------------------------------
* The images were of different size(different aspect ratio), and the features were not uniformly distributed over the image.
* The training data set was less as compared to the test data, which required the model to generalize well.
* The hardware bottleneck in training when we augment and enlarge the dataset manually.

Our fix to the above challenges:
-------------------------------- 
* Using a custom-designed padding technique and a few hand-designed data cleaning functions using OpenCV.
* Using keras ImageDataCenter class to augment and enlarge the dataset so that the model generalizes well.
* The last challenge was taken care of by training multiple models simultaneously in Google Colab platform.

Our model Architecture:
-----------------------
* Our model was a custom implementation hugely inspired from the famous AlexNet architecture with major improvisations and tweaks to serve our specific purpose

Or Training Strategy:
---------------------
* We trained our model on the enlarged dataset, for a total of 30 to 40 epochs, wherein the learning rate was decayed for every ten epochs.

The [VISTA82.ipynb file](https://github.com/nishantkr18/Vista-Codefest-2k19/blob/master/VISTA82.ipynb) contains the source code.
