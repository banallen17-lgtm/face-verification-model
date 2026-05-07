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
