# Caption-to-Image-Generation

## Overview
This project implements a caption-to-image generation model to genrate images from custom captions. **Stable Diffusion** model—a powerful latent diffusion model, a kind of deep generative artificial neural network. Stable Diffusion is known for generating high-quality images based on textual input by leveraging a diffusion process.

## Dataset
Used open-source **Flickr30k** dataset, which contains 31,000 images with five captions each, describing various scenes. 
The dataset is structured into:
- `caption_0`, `caption_1`, `caption_2`, `caption_3`, `caption_4`: Different captions for each image.
- `image`: Corresponding images for each set of captions.

## Stable Diffusion
**Stable Diffusion** is a pre-trained text-to-image model that generates images using a process of iterative noise reduction. It operates by gradually refining random noise into coherent images, conditioned on text descriptions. 

Key features of the Stable Diffusion model:
- **Diffusion Process**: The model gradually denoises random images in a process governed by a latent variable model, transforming noise into visually accurate images.
- **Flexibility**: Capable of generating diverse and detailed images, Stable Diffusion can be used for comparison and benchmarking alongside our custom-built model.

## Results
Below are some sample outputs:

Caption: A busy promenade where people gather
<p float ="left"> 
  <img src="Output/(Actual) A busy promenade where people gather.PNG"/><figcaption>Actual from Dataset</figcaption>
  <br><br><img src="Output/A busy promenade where people gather.PNG"/> <figcaption>Generated</figcaption>
</p>

Caption: A futuristic city with flying cars at night with neon lights
<p align="center">
  <img src="Output/A futuristic city with flying cars at night with neon lights.PNG"/>
</p>

Caption: A laughing robot in the sunset
<p align="center">
  <img src="Output/A laughing robot in the sunset.PNG"/>
</p>

Caption: A majestic mountain landscape with a sunset sky and a flowing river in the foreground and players playing soccer
<p align="center">
  <img src="Output/A majestic mountain landscape with a sunset sky and a flowing river in the foreground and players playing soccer.PNG"/>
</p>

## Future Improvements
Fine-tuning the custom model with more advanced architectures.
Exploring further integration with Stable Diffusion to improve image quality.
Experimenting with larger datasets to enhance model generalization.
