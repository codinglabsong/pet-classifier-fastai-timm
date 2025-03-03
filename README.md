# Simple Pet Classifier 🌖

A web application that classifies pet breeds from an input image using deep learning. This app uses Hugging Face Spaces, Fast.ai, Gradio, and timm to deliver real-time predictions.

---

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation and Setup](#installation-and-setup)
- [Usage](#usage)
- [Example Output](#example-output)
- [Links](#links)
- [License](#license)
- [Acknowledgements](#acknowledgements)

---

## Overview

**Simple Pet Classifier** allows users to upload an image of a pet and receive a predicted breed. Whether you're a pet owner, veterinarian, or just curious, this app demonstrates how deep learning can be applied to image classification tasks.

---

## Features

- **Image Classification:** Upload an image and get a probability distribution for various pet breeds.
- **Real-Time Inference:** Powered by Gradio for live, interactive predictions.
- **Easy Deployment:** Hosted on Hugging Face Spaces for seamless sharing.
- **Lightweight Codebase:** Built with Fast.ai and timm for efficient training and prototyping.

---

## Technologies Used

- **Hugging Face Spaces** for hosting the live app.
- **Fast.ai** for rapid model training.
- **Gradio** for building the interactive user interface.
- **timm** for pre-trained deep learning architectures.
- **Jupyter Notebook** for development and experimentation.

---

## Installation and Setup

### Clone the Repository

```bash
git clone https://github.com/codinglabsong/simple_pet_classifier.git
cd simple_pet_classifier
```

### Create and Activate a Virtual Environment

```bash
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate
```

### Install Required Packages

```bash
pip install -r requirements.txt
```
Note: If you work with large files locally, ensure Git LFS is set up as needed.

## Usage

### Running the App Locally

1. Download the Pre-trained Model: Download the model from the [v1.0.0 release](https://github.com/codinglabsong/simple_pet_classifier/releases/tag/v1.0.0) and place model.pkl in the project directory.

2. Start the Application:
```bash
python app.py
```
The Gradio interface will launch in your browser.

## Deploying on Hugging Face Spaces
This repository is configured for deployment on Hugging Face Spaces. Visit the live app here:

[Hugging Face Spaces App](https://huggingface.co/spaces/codinglabsong/simple_pet_classifier)

## Example Output
Below is an example output from the model when processing an image:

```python
{
  'Abyssinian': 1.1833922997084301e-07,
  'Bengal': 3.624234352628264e-07,
  'Birman': 4.868387648571115e-08,
  'Bombay': 2.7620779974313336e-07,
  'British_Shorthair': 1.1813022560147601e-08,
  'Egyptian_Mau': 1.5571941958114621e-06,
  'Maine_Coon': 3.696516159834573e-07,
  'Persian': 1.697121660981793e-06,
  'Ragdoll': 4.783786522466471e-08,
  'Russian_Blue': 1.0520943050096321e-07,
  'Siamese': 1.8542475288541027e-07,
  'Sphynx': 1.737347865571337e-08,
  'american_bulldog': 6.320234557932736e-09,
  'american_pit_bull_terrier': 7.586324812791645e-08,
  'basset_hound': 0.9999231100082397,
  'beagle': 5.7861499954015017e-05,
  'boxer': 4.267499065235825e-08,
  'chihuahua': 3.4804895676643355e-07,
  'english_cocker_spaniel': 4.314403213356854e-06,
  'english_setter': 5.8502276800709296e-08,
  'german_shorthaired': 1.6395551938330755e-06,
  'great_pyrenees': 1.0636112790507468e-07,
  'havanese': 9.475484574750226e-08,
  'japanese_chin': 6.481283776338387e-08,
  'keeshond': 6.536837418025243e-07,
  'leonberger': 9.268669742823477e-08,
  'miniature_pinscher': 1.3982798918732442e-07,
  'newfoundland': 1.264948963353163e-07,
  'pomeranian': 1.947668977209105e-07,
  'pug': 1.1417224641263601e-06,
  'saint_bernard': 5.6963376238172714e-08,
  'samoyed': 3.751043209376803e-08,
  'scottish_terrier': 4.281065230316017e-06,
  'shiba_inu': 2.990866221352917e-08,
  'staffordshire_bull_terrier': 8.163000053684755e-09,
  'wheaten_terrier': 2.0252580057444902e-08,
  'yorkshire_terrier': 7.572912750219984e-07
}
```
Note: In this example, the 'basset_hound' probability is near 1, indicating the model's high confidence in that classification.

## Links
Hugging Face Spaces App:
https://huggingface.co/spaces/codinglabsong/simple_pet_classifier

Pre-trained Model Release:
https://github.com/codinglabsong/simple_pet_classifier/releases/tag/v1.0.0

## License
This project is licensed under the [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0).

## Acknowledgements
- Thanks to the communities behind [Fast.ai](https://www.fast.ai/), [Gradio](https://gradio.app/), [timm](https://github.com/rwightman/pytorch-image-models), and [Hugging Face](https://huggingface.co/) for their invaluable tools and support.
- This project was inspired by the [Fast.ai Course](https://course.fast.ai/).
- Special thanks to contributors and reviewers who help improve this project.