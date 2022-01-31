# Python-kNN
kNN Python Example (Jupiter Notebook)

This is an example code for k-NN implemented in python (Jupyter notebook).
This simple program was designed to perform image segmentation.
It needs a training image (i.e. pyramid2.jpeg), a labelled image (pyramid2_label.jpeg), and a test image (pyramid1.jpeg).
3 example images are also included in this repository.
As you can see in the example labelled image, areas of the image are labelled with 3 different colors (namely Red, Green Blue).
The program will read the labels based on these 3 colors. 
The k-NN training is relatively simple (it randomly picks 100 samples to form the k-NN).
To segment the image, each pixel is then compares with the training set and find the k training samples with the closest  Euclidean distance with this pixel (i.e. in the R,G,B space). It then labels the pixel with the label with the majority vote in these k samples (i.e. majority of the samples are with this label).
The program will go through pixel by pixel and segment the image accordingly.
