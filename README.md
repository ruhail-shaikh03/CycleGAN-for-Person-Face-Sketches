# CycleGAN for Person Face Sketches

This project implements the CycleGAN model for image-to-image translation between real person face images and their corresponding sketches. The goal is to train a model that can:
1.  Convert a real face image into a sketch.
2.  Convert a sketch into a realistic face image.

The implementation is based on the original CycleGAN paper: "Unpaired Image-to-Image Translation using Cycle-Consistent Adversarial Networks" by Zhu et al.

## Dataset

The model is trained on the **Person Face Sketches dataset** available on Kaggle:
[https://www.kaggle.com/datasets/almightyj/person-face-sketches](https://www.kaggle.com/datasets/almightyj/person-face-sketches)

This dataset contains two domains:
*   `domain_a`: Real face images.
*   `domain_b`: Corresponding sketches of those faces.
(Note: While CycleGAN handles unpaired data, this dataset structure is convenient. Ensure your data loader handles these as separate domains A and B).

## Objectives Met

*   Implementation of the CycleGAN model.
*   Image-to-image translation:
    *   Face image → Sketch
    *   Sketch → Face image
*   End-to-end training.
*   Model weights are saved after every epoch to allow resuming training.

## Project Structure (Example)
