# FaceRecognition
Developed a FaceNet-based system for office security, allowing entry without ID cards via face verification and recognition

# Features
- Implemented one-shot learning with triplet loss to encode face images into 128-dimensional vectors.
- Utilized a ConvNet to compute encodings.
- Applied the triplet loss function to push the encodings of the same person (Anchor and Positive) closer and pull the encodings of different persons (Anchor and Negative) apart.
- Used a pretrained FaceNet model to minimize triplet loss, due to high data and computation requirements for training.
- Developed a face verification and recognition system with a database mapping names to face embeddings.
- Built a face verification database containing one encoding vector for each authorized person to check if the person at the door matches the name on the ID.
- Implemented a face recognition system to identify authorized persons from an input image without needing a name as input.
- Utilized the same encoding for both verification and recognition by measuring distances between two images encodings to determine if they depict the same person.