# AES Block Cipher Modes Analysis

<p align="center">
  <img src="Images/Banner.jpg" width="1100">
</p>

## Overview
This project analyzes AES block cipher modes through practical OpenSSL experiments and image encryption. The comparison demonstrates how ECB leaks plaintext patterns while CBC obscures image structure through chaining and IV usage.

## Environment Setup
Experiments were performed in a Linux virtual machine using OpenSSL and Jupyter Notebook.

## Experiments
### ECB Image encryption
AES in ECB mode revealed repeating image patterns.

### CBC Image encryption
CBC used an IV and block chaining to hide visible structure.

### IV behavior analysis
Initialization Vectors (IVs) were analyzed to demonstrate their role in preventing identical plaintext from producing identical ciphertext across multiple encryptions. When a random IV is used, the same input can generate different ciphertext outputs each time. This improves confidentiality and prevents pattern reuse.

### Additional mode comparisons

