# k-means.py
Python implementation of Lloyd's k-means clustering algorithm for image segmentation.

Using PIL, this program will load a selected image, and analyze pixel-by-pixel the RGB values to find the centroid values of the image. Once the centroid values have been found, the program will the produce and display the segmented image with the found RGB centroid values.

K-number of centroids are initialized randomly with in the min and max RGB values of the image.

Since this program executes the clustering algorithm in a serialized pixel-by-pixel basis, runtime of this program is slower with larger resolution pictures. Also as of now, program only runs with the selected test `.jpg` images in the `img` folder.

## USE

Simply exectute `k-means.py` with with the Python execution command, then enter a number between 1 and the number of images in the folder, and the k-value you wish to execute the program with:

```
../k-means.py>python k-means.py
Enter image number:
Enter K value:
```

Program will then run the program until centroid convergence is reached, then display the segmented image based on the found centroids.

![alt text](https://s4.postimg.org/77usarndp/k_means_image.png "k-means.py output image")