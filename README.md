# Face-anonymizer

In today’s technological world, where we have search engines like Clearview just for facial
recognition, it is important to restrict the accessibility to our faces and ensure the
fundamental right to privacy. This project is to work towards the anonymization of the faces
present in any live feed, captured videos, and photos. This was achieved by first detecting
the faces using the Haar Cascade algorithm and then turning the detected faces into a small
block for the data to be lost permanently and finally resizing it. Face Detection using Haar
feature-based cascade classifiers is an effective detection method used even today in various
places. The anonymization process is invariant to the movements and therefore, can keep
the face anonymous if it is in the frame.

We begin by accessing the camera live feed using CV2, an OpenCV package for Python. Next, using the Haar feature-based cascade classifier, faces are detected, and bounding boxes are created. The feature sets for the classifier are in the XML format and the window size for the attentional cascade is set as 24x24. The training data consists of both positive and negative images meaning the images that contain the faces and the images without any faces.The best way to truly ensure anonymity is to make sure that the faces within cannot be reconstructed. To do this, one solution is to use a blurring method that loses enough data that reconstruction becomes close to impossible. To ensure sufficient data loss, the section of the image inside the bounding box is transformed into an 8×8 image, and then changed back to its original resolution, and stitched to the original image

## Results

![image](https://user-images.githubusercontent.com/94932358/169161313-a3587e28-4c00-4269-bb1d-b24caf64fe8d.png)
![image](https://user-images.githubusercontent.com/94932358/169161325-aa322fa0-5502-4bc6-8eb8-9f5a22e6f39a.png)
![image](https://user-images.githubusercontent.com/94932358/169161340-be738a23-6007-4255-884f-79e5e422de14.png)
![image](https://user-images.githubusercontent.com/94932358/169161364-022eb354-82e9-4606-869a-45bdf3be91fb.png)

