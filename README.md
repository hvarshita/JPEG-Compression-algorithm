# JPEG Compression Algorithm for Image

This is a Python implementation of the JPEG compression algorithm for image compression. The Python notebook contains code for storing encoded image file that is compressed by 22 times the original size.. It uses Discrete Cosine Transform (DCT) and Huffman coding to achieve compression.

## Overview

JPEG (Joint Photographic Experts Group) is a widely used image compression standard. This implementation demonstrates the basic steps involved in JPEG compression:

1. **Discrete Cosine Transform (DCT)**: The image is divided into 8x8 blocks, and a 2D DCT is applied to each block. This helps to transform the image data into frequency components.

2. **Quantization**: The DCT coefficients are quantized using a predefined quantization matrix. Higher-frequency components are quantized more aggressively, leading to loss of data.

3. **Zigzag Scanning**: The quantized coefficients are scanned in a zigzag pattern to create a one-dimensional array. This is a step in preparing the data for entropy encoding.

4. **Huffman Encoding**: Huffman coding is applied to the quantized coefficients to represent them more efficiently. Huffman codes are generated for different coefficients based on their frequencies.

5. **Compression**: The compressed data is stored in a binary file format. The Huffman codes and quantization matrices are usually stored in the file header.

## Usage

1. Clone the repository to your local machine.
2. Ensure you have the required dependencies installed, including NumPy, SciPy, PIL (Pillow), and Matplotlib.
3. Run the provided Python script to perform JPEG compression on an input image.

