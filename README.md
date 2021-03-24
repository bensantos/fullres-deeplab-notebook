# fullres-deeplab-notebook
A modification of Deeplab's Colab Notebook that can generate segmentation maps the same size of the original image.

The original Deeplab repository provides a helpful Google Colab that lets you run inference and generate segmentation maps easily. Unfortunately, due to the architecture of the model, any test images are scaled down locked at a max resolution of 513 x 513. A solution is retraining the model, but I also found just rescaling the segmentation map using PIL worked well. It's not optimal, but it is not a bad start. 

I also added bonus compatibility for segmentation using the ADE20k dataset.
