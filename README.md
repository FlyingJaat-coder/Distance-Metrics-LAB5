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

<img width="1153" height="704" alt="image" src="https://github.com/user-attachments/assets/51e1202d-bc40-4c0a-92ed-570e11f1f365" />
<img width="718" height="387" alt="image" src="https://github.com/user-attachments/assets/362c5fd4-8b73-4bc0-adca-facdb527d1a7" />
<img width="716" height="381" alt="image" src="https://github.com/user-attachments/assets/2f7d0658-265c-4309-8257-f90d385a3298" />
<img width="351" height="387" alt="image" src="https://github.com/user-attachments/assets/42b51185-a7c3-4a26-ba85-f80d08084d44" />
<img width="714" height="385" alt="image" src="https://github.com/user-attachments/assets/2d7e152c-850c-4940-a154-a0b34ebb53fa" />
<img width="716" height="386" alt="image" src="https://github.com/user-attachments/assets/2cc01322-bf44-427b-b72d-f6ade8f4fe21" />





