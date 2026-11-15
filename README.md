# C++ Steganography Using Least Significant Bit (LSB) Technique

## Project Summary
This project implements image steganography using C++. It focuses on hiding secret information inside an image so that the presence of the message is not easily noticeable.

The project uses the **Least Significant Bit (LSB) technique** to embed secret data into image pixel values and retrieve the hidden information during decoding.

## Overview
Steganography is the technique of hiding confidential information inside another file, such as an image, audio file, or video, without creating an obvious indication that secret data exists.

In this project, an image acts as the cover medium, and secret data is embedded into its pixel information by modifying the least significant bits.

The changes made to the image are designed to be visually insignificant.

## Problem Statement
Transmitting confidential information directly can expose the existence of the message.

This project addresses that problem by hiding secret information inside an image, making the communication less noticeable.

## Technologies Used
- Programming Language: C++
- Concept: Image Steganography
- Technique: Least Significant Bit (LSB)
- Concepts: Bitwise Operations, File Handling, Binary Data Processing

## Methodology

### 1. Encoding
- Read the cover image.
- Read the secret message.
- Convert the message into binary representation.
- Embed the message bits into the least significant bits of the image pixel data.
- Generate the output image containing the hidden message.

### 2. Decoding
- Read the encoded image.
- Extract the least significant bits from the pixel data.
- Reconstruct the binary message.
- Convert the extracted binary data into readable text.

## Working Principle: LSB Technique
Each pixel component is represented using binary bits.

The least significant bit is modified to store secret information.

For example:

Original pixel value:
`10010110`

Secret bit:
`1`

Modified pixel value:
`10010111`

Only the last bit changes, so the visual difference is generally very small.

## Key Concepts Learned
- Bitwise operators in C++
- Binary data representation
- File handling
- Image data processing
- Encoding and decoding
- Data hiding techniques
- Memory and data manipulation

## Sample Workflow

**Encoding:**
Cover Image + Secret Message → LSB Encoding → Stego Image

**Decoding:**
Stego Image → LSB Extraction → Hidden Message

## How to Run

1. Clone the repository:

   ```bash
   git clone <repository-url>
   ```

2. Navigate to the project directory:

   ```bash
   cd <project-folder>
   ```

3. Compile the source files using the appropriate compiler command for your project.

4. Run the generated executable and follow the program instructions.

*Note: Update the compilation and execution commands according to your actual source-file structure and implementation.*

## Applications
- Confidential data communication
- Digital information hiding
- Secure image-based communication
- Educational study of binary data processing

## Future Improvements
- Support for different image formats
- Password-based message protection
- Encryption before embedding
- Support for larger secret messages
- Improved error detection during decoding

## Author
**Manjusha Thiruveedhula**

