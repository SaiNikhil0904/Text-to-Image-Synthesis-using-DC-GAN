# Text-to-Image Synthesis using DC-GAN

## Overview
Welcome to our Text-to-Image Synthesis project, where we use DC-GAN to transform textual descriptions into visually realistic images. Developed during our B.Tech program at BML Munjal University.

## Requirements
To run this project successfully, make sure you have the following prerequisites:
- Python, NumPy, Pandas, Keras
- Google Colab (optional, but recommended for faster GPU-based training)

## Dataset
Our exploration heavily relies on the [Oxford 102 Flower dataset](https://www.kaggle.com/datasets/nunenuh/pytorch-challange-flower-dataset), a comprehensive resource containing 8,192 images across 102 categories of flowers. Each image is associated with multiple captions, forming the foundation for our training data.

### Introduction
Text-to-image synthesis is a process of making a computer understand and create images from textual descriptions. In our project, we're exploring the task of generating beautiful flower images from user descriptions, bridging the world of words and pictures using computer vision techniques.

### Problem Statement
Generating realistic images from user input text is a challenging task in computer vision. This project aims to create a model capable of synthesizing 64-image size flower images from corresponding text descriptions. The challenging part is getting all the little details of flowers right by understanding the words users use, requiring a mix of understanding natural language processing and computer vision.

## Purpose
Our primary goal is to delve into the capabilities of DC-GAN for generating images from textual prompts. This project serves as a practical application of our theoretical knowledge, allowing us to bridge the gap between Natural Language Processing and Computer Vision.

### Data Preprocessing
The data preprocessing step involves organizing and processing the images into a binary file for efficient access. Captions are also processed into a binary file, saving caption embeddings using NumPy. This meticulous organization facilitates efficient training and testing processes.

### Methodology
#### Data Modeling
In this section, we work on core concepts of DC-GAN, defining the Generator and Discriminator functions. These functions use multiple activation functions to bring non-linearity into the implementation of the model.

#### Transfer Learning Challenges
Transfer learning, specifically in the context of text-to-image synthesis, can be challenging due to domain mismatch (source domain is NLP, and the target domain is image data) and the complexity of the task.

#### What is GAN (Generative Adversarial Network)?
GANs consist of two neural networks, the generator and the discriminator, engaged in an adversarial training process. The generator creates synthetic data, and the discriminator evaluates whether the generated data is real or fake. The continuous competition between these two networks results in the generation of increasingly realistic data.

#### Why Choose GAN for Text-to-Image Synthesis?
GANs are particularly well-suited for tasks like text-to-image synthesis due to their ability to learn complex, high-dimensional data distributions. In this project, GANs enable the generation of flower images from textual descriptions, effectively bridging the gap between text and image modalities.

#### Why Choose DCGAN?
DCGAN (Deep Convolutional Generative Adversarial Network) is a specific variant of GAN that incorporates convolutional layers in both the generator and discriminator networks. This convolutional architecture is crucial for handling image data, capturing spatial dependencies, and learning hierarchical features.

### Model Architecture
![Model Architecture](https://github.com/SaiNikhil0904/Text-to-Image-Synthesis-using-DC-GAN/assets/98106917/5365cc88-3056-4edb-ba41-57154f6ff8a9)

### Output/Result
![Output/Result](https://github.com/SaiNikhil0904/Text-to-Image-Synthesis-using-DC-GAN/assets/98106917/059b25bb-47cf-4868-8aa8-da8c258e8743)

## Key Features
- **DC-GAN Architecture:** Our model utilizes the GAN-CLS algorithm, a matching-aware discriminator, to generate images from text and image pairs. The deep convolutional architecture ensures the automatic learning of text representations.
- **GloVe Embedding:** To enhance the semantic understanding of captions, we incorporated GloVe Embedding, an unsupervised learning algorithm for obtaining vector representations for words.
- **Data Pre-processing:** We meticulously organized and pre-processed the dataset, including images and caption embeddings, facilitating an efficient training and testing process.
- **Training Process:** The model underwent rigorous training for over 1800 epochs. We observed a progressive improvement in image generation capabilities, showcasing the effectiveness of the GAN-CLS algorithm.

## Project Impact
While the generated images are of 64x64 resolution, our qualitative analysis indicates the model's growing accuracy in comprehending prompts and generating appropriate images. This project marks our initiation into the realm of generative AI models, motivating us to explore further applications and contribute to this dynamic field.

## Explore the Work
Feel free to explore our codebase, experimental results, and detailed learnings. Your engagement and feedback are highly valued as we continue refining and expanding our project.  Check out our [Colab Notebook](https://colab.research.google.com/drive/14j2jbeLtjV7C_RpAXAVkKSnikx2OaDZ0?usp=sharing).

## Team
- **Anish Borkar**
- **Godavarthi Sai Nikhil**

## Mentor
We extend our sincere gratitude to **Dr. Soharab Hossain Shaikh** for being our guiding force throughout this Deep Learning journey. His mentorship and insights have been instrumental in the success of our project.

## Contact Us

For inquiries, collaboration opportunities, or further information, please feel free to reach out to us:

Godavarthi Sai Nikhil: nikhilgodavarthi9@gmail.com

Anish Borkar: anishborkar73@gmail.com

Thank you for joining us on this exciting journey of Text-to-Image synthesis using DC-GAN!
