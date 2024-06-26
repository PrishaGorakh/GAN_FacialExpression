# GAN_FacialExpression
Generating different facial expressions.  
This project utilizes Generative Adversarial Networks (GANs) to generate lifelike facial images based on various expressions. This project employs two different types of GAN architectures: Conditional GANs (cGANs) and Auxiliary Classifier GANs (ACGANs), to create diverse and expressive faces.   
## Introduction  
Facial expression generation has long been a challenging task in the field of computer vision and artificial intelligence. We aim to overcome this challenge by leveraging the power of GANs, a class of machine learning algorithms that excel at generating realistic data samples.  
## Objective
The objective of this project is to utilize Generative Adversarial Networks (GANs), to generate synthetic facial images corresponding to different emotional expressions (e.g., happy, neutral, sad, angry, fear, surprised, disgust).  
1.Utilize Conditional Generative Adversarial Networks (CGANs) and Auxiliary Classifier Generative Adversarial Networks (ACGANs) to generate realistic black and white facial images.  
2.Incorporate specific emotion labels (happy, neutral, sad, angry, fear, surprised, disgust) to guide the generation process, enabling the creation of diverse facial expressions.  
3.Train the GAN models on the fer2013 dataset to develop a system capable of synthesizing expressive facial images corresponding to different emotions, advancing research in emotion recognition and synthesis.  
## Flowchart  
<p align="center">
<img width="861" alt="Screenshot 2024-05-02 at 8 40 51 PM" src="https://github.com/PrishaGorakh/GAN-RMFC-Div-A-FacialExpression/assets/124128845/b45c1326-a309-4456-889e-f115da2f43a9">
</p>

## Architecture  
We have used two primary architectures for expression-based facial image generation:  
**Conditional GAN (cGAN):** In this architecture, the generator takes both a random noise vector and a conditional label representing the desired expression as input. The discriminator evaluates the generated images based on both their realism and whether they match the specified expression label.
<p align="center">
<img width="389" alt="Screenshot 2024-05-03 at 2 35 21 PM" src="https://github.com/PrishaGorakh/GAN-RMFC-Div-A-FacialExpression/assets/124128845/f9699419-ef88-4364-9545-eb58d578713d">
</p>

**Auxiliary Classifier GAN (ACGAN):** ACGAN extends the cGAN architecture by introducing an auxiliary classifier in the discriminator. This classifier not only distinguishes between real and fake images but also predicts the expression label associated with the generated images.  
<p align="center">
<img width="389" alt="Screenshot 2024-05-03 at 2 34 15 PM" src="https://github.com/PrishaGorakh/GAN-RMFC-Div-A-FacialExpression/assets/124128845/26f39053-2cb4-4230-881a-d0b688a3bf77">
</p>

## Datasource:  
Dataset contain a CSV file of black and white labeled 48x48 images from the FER2013 dataset. Data contains 35,887 records from Fer2013:   
14,685 - Happy (29.63%) Emotion: 3  
13,066 - Neutral (26.36%) Emotion: 6  
6,345 - Sad (12.8%) Emotion: 4  
5,205 - Angry (10.5%) Emotion: 0  
5,142 - Fear (10.37%) Emotion: 2  
4,379 - Surprised (8.82%) Emotion: 5  
755 - Disgust (1.52%) Emotion: 1  
The CSV contains 3 columns Emotion, Pixels and Usage.  
(https://www.kaggle.com/datasets/nicolejyt/facialexpressionrecognition)  
## Conclusion  
The project successfully leverages Conditional Generative Adversarial Networks (CGANs) and Auxiliary Classifier Generative Adversarial Networks (ACGANs) to generate realistic black and white facial images corresponding to specific emotion labels. By training these models on the fer2013 dataset, the system achieves the objective of synthesizing diverse and expressive facial expressions. Through rigorous evaluation, analysis, and optimization, the project demonstrates the effectiveness of GANs in generating high-quality facial images with fine-grained control over emotions.  
## Refrences  
https://www.kaggle.com/datasets/nicolejyt/facialexpressionrecognition  
https://machinelearningmastery.com/how-to-develop-a-conditional-generative-adversarial-network-from-scratch/  
https://machinelearningmastery.com/how-to-develop-an-auxiliary-classifier-gan-ac-gan-from-scratch-with-keras/  
https://www.geeksforgeeks.org/conditional-generative-adversarial-network/
