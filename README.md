# Image Filter

##Image Processing

A general image processing operator is a function that takes one or more input images and produces an output image.
Image transforms can be seen as:
Point operators (pixel transforms)
Neighborhood (area-based) operators

## Brightness and contrast adjustments

Two commonly used point processes are multiplication and addition with a constant:

          g(x)=af(x)+ß

The parameters a>0 and ß are often called the gain and bias parameters.
sometimes these parameters are said to control contrast and brightness respectively.
You can think of f(x) as the source image pixels and g(x) as the output image pixels. 
Then, more conveniently we can write the expression as:

          g(i,j)=a·f(i,j)+ß
where i and j indicates that the pixel is located in the i-th row and j-th column.

##Convolution

Convolution is the process of adding each element of the image to its local neighbors,
weighted by the kernel. This is related to a form of mathematical convolution. 
It should be noted that the matrix operation being performed - convolution - is not 
traditional matrix multiplication, despite being similarly denoted by *.