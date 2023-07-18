# How to take an image and ask our application to replace an object in that image with something else.

3 individual models that work together to solve a problem that was near impossible months ago.  

The example uses the following:  

• A Zero-Shot Object Detection model  
• A Segmentation model  
• A Diffusion model  

Let me show you:

We want to take an image and ask our application to replace an object in that image with something else.  

For example:  

• We show it an image of a fox.  
• And we tell it to replace the fox with a dog.  

The output should be the same image with a dog instead of a fox.  

![Image of fox](img/fox.jpg)

To solve this problem, we can create a pipeline using the following models:  

• Grounding DINO for object detection  
• Segment Anything for segmentation  
• Stable Diffusion to do the painting  

(The full tutorial and source code is at the end of this post.)  

Grounding DINO is a zero-shot object detector.  

It's pretty nuts!  

You give the model a prompt and an image, and it will return bounding boxes around that object on the image.  

We call it "zero-shot" because it can identify objects even if they are not part of the training data.  

The second model in the pipeline will be @MetaAI's Segment Anything Model (SAM).  

It's also zero-shot and capable of segmenting objects on an image even when those objects weren't part of the training data.  

SAM was released earlier this year.  



