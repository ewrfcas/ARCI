## LeftRefill: Filling Right Canvas based on Left Reference through Generalized Text-to-Image Diffusion Model (CVPR2024)


[Project Page](https://ewrfcas.github.io/LeftRefill/)


## Abstract

This paper introduces LeftRefill, an innovative approach to efficiently harness large Text-to-Image (T2I) diffusion models for reference-guided image synthesis. 
As the name implies, LeftRefill horizontally stitches reference and target views together as a whole input. 
The reference image occupies the left side, while the target canvas is positioned on the right.
Then, LeftRefill paints the right-side target canvas based on the left-side reference and specific task instructions. 
Such a task formulation shares some similarities with contextual inpainting, akin to the actions of a human painter.

This novel formulation efficiently learns both structural and textured correspondence between reference and target without other image encoders or adapters.
We inject task and view information through cross-attention modules in T2I models, and further exhibit multi-view reference ability via the re-arranged self-attention modules.
These enable LeftRefill to perform consistent generation as a generalized model without requiring test-time fine-tuning or model modifications.
Thus, LeftRefill can be seen as a simple yet unified framework to address reference-guided synthesis. 
As an exemplar, we leverage LeftRefill to address two different challenges: reference-guided inpainting and novel view synthesis, based on the pre-trained StableDiffusion.


Codes and models will be released in
https://github.com/ewrfcas/LeftRefill.