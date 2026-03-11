# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

This is a university lab exercise (Week 8) on **Responsible AI — Saliency Maps** for explaining image classification models. The main artifact is a Jupyter notebook designed to run in Google Colab.

## Structure

- `w8_lab 2/Responsible_AI_Lab_Saliency_maps.ipynb` — Main notebook demonstrating Gradient and SmoothGrad saliency methods using the PAIR Saliency Library
- `w8_lab 2/*.jpg`, `w8_lab 2/*.png` — Test images (doberman, kitten/dog variants with perturbations)

## Key Technologies

- **TensorFlow/Keras** with pre-trained ImageNet models (VGG16, ResNet50)
- **PAIR Saliency Library** (`saliency.core`) for computing saliency masks
- Images are resized to 224x224; each model requires its own preprocessing function (e.g., `tf.keras.applications.vgg16.preprocess_input`)

## Architecture Notes

- `call_model_function` is the bridge between PAIR's saliency API and the Keras model — it handles gradient computation via `tf.GradientTape`
- When switching models, both the model object and the `PreprocessImage` function must be updated to match
- The notebook overwrites the global `model` variable when loading ResNet50, so cells must be run in order
