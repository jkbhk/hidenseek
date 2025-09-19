##This tool allows the user to hide a file inside an image.

## How does this work?
        
This is achieved using a combination of **AES encryption** and **image steganography**.
It first converts a selected file to base64, then AES encryption is performed on the string.
The encrypted string is then encoded in a PNG of suitable size using **naive Least Significant Bit(LSB)** steganography.

Assuming the original image contains enough noise, the resulting encoded image should be visually indistinguishable from the original.
