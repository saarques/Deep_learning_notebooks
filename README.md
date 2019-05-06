# Skin Cancer Detection For AI Without Border

## Task: Visualise Intermediate weights in a neural network fed with the skin cancer sample images.

## Input : The sample images from the input may look like this

![alt text](https://github.com/saarques/Deep_learning_notebooks/blob/master/Sample_input_images/Skin_cancer_input_image-10.png "Sample Input images")


## Output : The output weights may look like follow

Since the output weight concentrations were expected in the heatmap form, we've used "plasma" mapping for the concentration.

![alt text](https://github.com/saarques/Deep_learning_notebooks/blob/master/Sample_output_images/output_image_test0%200-11.jpg "Weight Concentration")

![alt text](https://github.com/saarques/Deep_learning_notebooks/blob/master/Sample_output_images/output_image_test0%201-29.jpg "Weight Concentration")

Other sample images may be found in the respective folders.

## Approach:
### Steps
 1. I've used Tensorflow in the backend with Keras to train the model with the help of convolutional neural networks which are the popular approach on such type of data.

 2. To initiate any work, one needs more and more information about the data to be used, so I did the same and studied various types of cancer cells present.

 3. After data wrangling and analysis, I created the model in this order [Conv2D -> relu]*2 -> MaxPool2D -> Dropout]*2 -> Flatten -> Dense # -> Dropout -> Out

 4. After creating the model, we simply needed to train it on the input images.

 5. Now, after training the model, we created a function named "save_image()" to visualise the weight concentrations with "plasma" mapping. 

 6. After all the steps, the weight concentrations are ready as output.