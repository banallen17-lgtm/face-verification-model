# face-verification-model
A face verification model that compares two face images and predicts whether they belong to the same person.

## Overview
This project is a face verification model that compares two uploaded face images and predicts whether they belong to the same person.

Unlike face classification, which tries to identify a person from a known dataset, face verification focuses on comparing two faces and determining whether they match.

## Features
- Upload two face images
- Extract face embeddings using a pretrained FaceNet model
- Compare embeddings using cosine similarity or distance
- Predict whether the two images show the same person
- Adjustable similarity threshold

## Technologies Used
- Python
- PyTorch
- facenet-pytorch
- NumPy
- PIL
- scikit-learn
- Google Colab

## How It Works
1. Two face images are uploaded.
2. A pretrained FaceNet model converts each face into a numerical embedding.
3. The embeddings are compared using a similarity score.
4. If the similarity score passes the threshold, the model predicts that the faces are the same person.

## Installation
```bash
pip install -r requirements.txt

## Dataset

This project was developed and tested using the VGGFace2 dataset, a large-scale face recognition dataset containing a wide variety of identities, poses, lighting conditions, and facial expressions.

The dataset was used to experiment with face embeddings and similarity comparison between images. Due to the large file size and licensing restrictions, the dataset is not included in this repository.

Dataset source:
https://www.robots.ox.ac.uk/~vgg/data/vgg_face2/

## Results

The model successfully compares two face images by converting them into numerical embeddings and calculating their similarity score.

When two images belong to the same person, the similarity score is generally higher. When the images belong to different people, the similarity score decreases significantly.

The project demonstrated effective face verification performance under normal lighting and clear facial visibility. Performance may vary depending on image quality, angle, facial obstruction, and lighting conditions.

## Limitations

- Verification accuracy may decrease when images are blurry, low quality, or poorly lit.
- Large differences in facial angle or facial expression can affect similarity scores.
- The model may struggle with partially covered faces or extreme lighting conditions.
- The verification threshold may require adjustment depending on the dataset or use case.
- This project focuses on verification between two images rather than full facial identification across large databases.

## Future Improvements

- Add real-time webcam face verification.
- Improve face detection and image preprocessing before embedding generation.
- Experiment with different pretrained face recognition models.
- Build a graphical user interface or web application for easier interaction.
- Optimize the model for faster real-time performance.
- Evaluate performance on larger and more diverse datasets.
- Add automatic threshold calibration for improved verification accuracy.
