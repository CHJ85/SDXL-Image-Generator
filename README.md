# SDXL-Image-Generator
This bash script makes it easy to generate high quality images using Stable Diffusion, without the need for a beefy graphics card.
My script provides an easy to use UX.
Your images will automatically open up in your default web browser after they're done generating.

# Recommended settings
My preset should work fine in most instances and provides a good starting point.
Here's a quick rundown.

Scheduler: Choose DDIM for general-purpose image generation. This scheduler often provides good results across various prompts and conditions.
Number of Inference Steps: Setting this to 50 is a reasonable default. It allows for sufficient denoising and refinement without excessively prolonging the processing time.
Guidance Scale: A value around 7.5 is often a good starting point. Adjust this based on how much guidance you want to provide to the AI model without overly influencing the output.
Prompt Strength: 0.8 strikes a balance where the prompt influences the output while allowing for some creative interpretation by the AI model. You can adjust this to fine-tune how strongly the input prompt affects the image generation.
Seed: Leave this blank to allow the system to randomize the seed. This helps in generating diverse outputs for the same prompt, useful for exploring different creative variations.
Refine Style: Depending on the specific use case:
    no_refiner: For basic image generation without additional refinement.
    expert_ensemble_refiner: Useful when you want to incorporate ensemble techniques for improved quality, especially when generating complex or detailed images.
    base_image_refiner: Suitable when refining based on a base image, useful in scenarios where you need to refine the generated output further.
High Noise Fraction: 0.8 is a balanced setting for adding noise, which can sometimes enhance the realism or diversity of generated images without overwhelming the output with noise artifacts.
Refine Steps: Defaults to 50, aligning with the number of inference steps unless specified otherwise. This parameter controls how many refining steps are applied, impacting the final quality and detail in the generated images.
