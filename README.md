AIM

The aim of this lab was to detect faces in an image and group them using clustering techniques. We used OpenCV for face detection and applied K-Means clustering based on color features. We also tested the model by predicting which cluster a new image belongs to.


METHODOLOGY

First, we loaded the group image using OpenCV. The image was converted to grayscale because face detection works better on grayscale images. We then used the Haar Cascade classifier to detect faces. After detection, rectangles were drawn around each face and we counted the total number of faces found.

Next, we converted the original image into HSV color space. For each detected face, we calculated the average Hue and Saturation values. These values were used as features for clustering.

We then applied K-Means clustering with 3 clusters to group the faces based on their HSV values. The clusters were visualized using a scatter plot to understand how the faces were separated.

Finally, we loaded a template image, detected the face in it, extracted its HSV features, and used the trained K-Means model to predict which cluster it belongs to.


KEY FINDINGS

- The Haar Cascade classifier was able to detect multiple faces successfully.
- Hue and Saturation values helped in grouping faces based on color similarity.
- K-Means clustering divided the faces into three groups.
- The scatter plot made it easier to visualize the clusters.
- The template image was successfully classified into one of the clusters.


CONCLUSION

From this lab, we understood how face detection and clustering can work together. We learned how to use OpenCV for detecting faces and how to extract simple image features for machine learning. Even though we only used basic color features, the clustering results were reasonable. This experiment helped in understanding practical applications of computer vision and unsupervised learning.
