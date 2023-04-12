# Image-Augmentation
This code performs data augmentation on an image using the Albumentations library in Python. 

The visualize() function is defined to display the image using Matplotlib.

The first line loads an image from a file path using the OpenCV library and assigns it to the variable image. 

The visualize() function is then called to display the original image.

The transform variable defines a series of image augmentation operations using the A.Compose() function. 

A.Compose() function to create a pipeline of image augmentation operations. 

The Compose function is a class in the Albumentations library that allows us to chain multiple image augmentation operations together.

By using the A.Compose() function, we can define a series of image augmentation operations to be applied to an input image in a specific order. Each operation can be defined using a specific class in the Albumentations library, such as HorizontalFlip, Resize, RandomRotate90, and so on.

These operations include:
1)HorizontalFlip(): flips the image horizontally with a 90% probability (p=0.9)
2)VerticalFlip(): flips the image vertically with a 70% probability (p=0.7)
3)Resize(): resizes the image to a height of 106 pixels and a width of 160 pixels using nearest neighbor interpolation
4)RandomRotate90(): randomly rotates the image by 90 degrees
5)HueSaturationValue(): randomly changes the hue, saturation, and value of the image
6)InvertImg(): inverts the colors of the image

The transform() function is then called on the original image image using the transform variable as an argument. The transformed image is stored in the variable augmented_image.

Finally, the visualize() function is called again to display the transformed image using Matplotlib.
