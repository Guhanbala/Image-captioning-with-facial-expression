# Image Captioning with Facial Expression Recognition

## Overview

Image Captioning with Facial Expression Recognition is a deep learning-based project that generates enhanced, context-aware captions for images containing human faces. Unlike conventional image captioning systems that describe only the visual elements in an image, our approach incorporates facial emotion recognition to understand the emotional context and generate more expressive and meaningful captions.

The system integrates facial emotion detection, an image captioning model, and GPT-2-based natural language processing to produce captions that reflect both the visual content and the emotions portrayed by individuals.

The project explores the implementation and integration of pretrained models and custom deep learning architectures using the available computational resources.

## Key Features

- **Facial Emotion Detection:** Identifies whether the emotion portrayed by a human face is happy or sad.
- **Real-Time Emotion Recognition:** Detects facial expressions through a real-time camera feed.
- **Custom Image Captioning Model:** Implements an encoder-decoder-based image captioning architecture.
- **Transformer-Based Caption Generation:** Uses a Transformer decoder to generate descriptive captions.
- **Emotion-Aware Caption Enhancement:** Integrates detected emotions with generated captions using GPT-2.
- **Natural Language Processing:** Produces more expressive and contextually enhanced captions with an extended output length of up to 30 words.

## Project Architecture

The project consists of three major components:

1. Facial Emotion Detection
2. Image Captioning Model
3. NLP-Based Caption Enhancement using GPT-2

### 1. Facial Emotion Detection

The emotion detection module is built using a Convolutional Neural Network (CNN).

- Extracts facial features from input images or a real-time camera feed.
- Processes the extracted facial features to classify the expression.
- Identifies two primary emotional categories: **Happy** and **Sad**.
- Provides the detected emotion as contextual information for the caption enhancement module.

### 2. Image Captioning Model

The image captioning module follows an Encoder-Decoder architecture combining CNN-based feature extraction and Transformer-based sequence generation.

**Encoder – CNN:**
- Uses a Convolutional Neural Network to extract meaningful visual features from the input image.
- Converts the extracted features into a feature representation (feature vector).
- Passes the visual representation to the Transformer decoder.

**Decoder – Transformer:**
- Takes the extracted image features as input.
- Generates captions sequentially by predicting the next word based on the image representation and previously generated words.
- Uses Softmax-based probability distribution to select the next word during caption generation.

This architecture enables the model to understand image content and generate descriptive natural-language captions.

### 3. NLP-Based Caption Enhancement (GPT-2)

The final component integrates the outputs from the emotion detection and image captioning modules using GPT-2.

- Takes the generated image caption and detected facial emotion as inputs.
- Combines visual descriptions with emotional context.
- Uses GPT-2 to refine and enhance the generated caption.
- Produces a more expressive and context-aware caption with an extended word limit of up to 30 words.

This integration helps the system move beyond basic object descriptions and generate captions that better represent the emotional context of an image.

## Technologies Used

- **Programming Language:** Python
- **Deep Learning:** TensorFlow / PyTorch, CNN
- **Computer Vision:** OpenCV
- **Image Captioning:** CNN Encoder, Transformer Decoder
- **Natural Language Processing:** GPT-2
- **Techniques:** Feature Extraction, Facial Emotion Recognition, Sequence Generation

## Research Publication

The project also resulted in a published research paper in IEEE, documenting the proposed approach and research contributions.

**Research Paper:** [Image Captioning with Facial Expression Recognition – IEEE Xplore](https://ieeexplore.ieee.org/document/11410892)

## Contributors

- [Guhan Balachandran](https://github.com/Guhanbala)
- [Jeevakamal K R](https://github.com/kamaladhi)
- [Shatha Varsha](https://github.com/ShathaVarsha)
- [Gowtham S D](https://github.com/GowthamDhanaraju)
