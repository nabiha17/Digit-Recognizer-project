![MINST_DIgit Recognizer](README_Images/MINST.png "MINST_DIgit Recognizer")

# Digit-Recognizer
> Implementing computer vision fundamentals with the famous MNIST data

MNIST ("Modified National Institute of Standards and Technology") is the de facto “hello world” dataset of computer vision. Since its release in 1999, this classic dataset of handwritten images has served as the basis for benchmarking classification algorithms. As new machine learning techniques emerge, MNIST remains a reliable resource for researchers and learners alike. This project aims to accurately identify digits from a collection of tens of thousands of handwritten images.

The programming language used in this project is <ins>Python</ins>, and the development environment is <ins>Google Colab</ins>.

<hr>

## Data Description:

The data files train.csv and test.csv contain grayscale images of hand-drawn digits, from zero through nine.

Each image is 28 pixels in height and 28 pixels in width, totaling 784 pixels. Each pixel has a single pixel-value associated with it, indicating the lightness or darkness of that pixel, with higher numbers meaning darker. This pixel-value is an integer between 0 and 255, inclusive.

The training dataset (train.csv) has 785 columns. The first column, called "label," is the digit drawn by the user. The remaining columns contain the pixel-values of the associated image.

Each pixel column in the training set has a name like pixelx, where x is an integer between 0 and 783, inclusive. To locate this pixel on the image, decompose x as x = i * 28 + j, where i and j are integers between 0 and 27, inclusive. Then, pixelx is located at row i and column j of a 28x28 matrix (indexing by zero).

```
000 001 002 003 ... 026 027
028 029 030 031 ... 054 055
056 057 058 059 ... 082 083
 |   |   |   |  ...  |   |
728 729 730 731 ... 754 755
756 757 758 759 ... 782 783
```

The test data set, (test.csv), is the same as the training set, except that it does not contain the "label" column.
