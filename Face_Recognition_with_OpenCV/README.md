# Face Recognition with OpenCV

To build our face recognition system, we値l first perform face detection, extract face embeddings from each face using deep learning, train a face recognition model on the embeddings, and then finally recognize faces in both images and video streams with OpenCV.

## Objectives
1) Detect faces
2) Compute 128-d face embeddings to quantify a face
3) Train a Support Vector Machine (SVM) on top of the embeddings
4) Recognize faces in images and video streams

## Files

1) extract_embeddings.py : It is responsible for using a deep learning feature extractor to generate a 128-D vector describing a face. All faces in our dataset will be passed through the neural network to generate embeddings.

2) openface_nn4.small2.v1.t7 : A Torch deep learning model which produces the 128-D facial embeddings.

3) train_model.py : Our Linear SVM model will be trained by this script in Step #2. We値l detect faces, extract embeddings, and fit our SVM model to the embeddings data.

4) recognize.py : We値l recognize faces in images. We値l detect faces, extract embeddings, and query our SVM model to determine who is in an image. We値l draw boxes around faces and annotate each box with a name.

5) recognize_video.py : Recognize people in a video.




