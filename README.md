# Project---Steganography-Tool-for-Image-File-Hiding
## Introduction
Image Steganography App  allows you to hide confidential text messages within images using the concept of steganography. Steganography is the art of hiding information within another seemingly innocuous medium, such as an image.

In this project, I utilized the power of Python and the tkinter library for creating the graphical user interface (GUI), and the stegano library for the steganography functionality. The app provides a user-friendly interface to encode text messages into images and decode hidden messages from images.

 ## Features
- Encode a text message into an image.
- Decode a hidden message from an image.
- Preview images before and after encoding/decoding.
- User-friendly GUI built with tkinter.
- Seamless integration with the stegano library for steganography operations.

## How to Use
- Clone this repository to your local machine.
- Make sure you have Python and the required libraries installed.
- Run the ImageCloak.py script:
- python ImageCloak.py
- The app window will open, providing options to encode and decode messages.
  
### To encode a message:
- Click on the "Open Image" button.
- Select the target image and provide the message you want to hide.
- Click "Save" to generate the encoded image.
  
### To decode a message:
- Click on the "Open Image" button.
- Select the image containing the hidden message.
- Click "Show Data" to reveal the hidden message.


### Features:
- compression of embedded data
- encryption of embedded data
- embedding of a checksum to verify the integrity of the extracted data
- support for JPEG, BMP, WAV and AU files

# Hide text/files in image using Kali linux:
Steghide is steganography program which hides bits of a data file in some of the least significant bits of another file in such a way that the existence of the data file is not visible and cannot be proven.


 
### Install Steghide:
      sudo apt update
     sudo apt install steghide

Prepare the Files:
- Choose the image file you want to use (e.g., cover.jpg).

- Prepare the file you want to hide (e.g., secret.txt).

### Embed the File Inside the Image:

     steghide embed -cf cover.jpg -ef secret.txt

It will prompt you to set a passphrase. This secures the hidden data.

### Verify the Embedding (Optional):

- To check if data is embedded:

       steghide info cover.jpg

### Extract the Hidden File Later:

      steghide extract -sf cover.jpg

Enter the passphrase to retrieve the hidden file.

### Result:

The file secret.txt will be extracted in the current directory.






