# Project---Steganography-Tool-for-Image-File-Hiding
### Introduction
Image Steganography App  allows you to hide confidential text messages within images using the concept of steganography. Steganography is the art of hiding information within another seemingly innocuous medium, such as an image.

In this project, I utilized the power of Python and the tkinter library for creating the graphical user interface (GUI), and the stegano library for the steganography functionality. The app provides a user-friendly interface to encode text messages into images and decode hidden messages from images.

### Requirements
- Python
- tkinter
- Pillow PIL 

### Features
- Encode a text message into an image.
- Decode a hidden message from an image.
- Preview images before and after encoding/decoding.
- User-friendly GUI built with tkinter.
- Seamless integration with the stegano library for steganography operations.
  
### Install Pillow (for image processing):
      
      pip install pillow

### How to Use:
- Clone this repository to your local machine.
  
- Make sure you have Python and the required libraries installed.
  
- Run the steganography.py script:

      python steganography.py
  
- The app window will open, providing options to encode and decode messages.

### To encode a message:
- Click on the "Open Image" button.
- Select the target image and provide the message you want to hide.
- Click "Save" to generate the encoded image.
  
### To decode a message:
- Click on the "Open Image" button.
- Select the image containing the hidden message.
- Click "Show Data" to reveal the hidden message.
  
### Project Output:

https://github.com/user-attachments/assets/fd0c1f96-7170-4886-b1a3-4cc471a3018f


# Hide text/files in image using Kali linux:
Steghide is steganography program which hides bits of a data file in some of the least significant bits of another file in such a way that the existence of the data file is not visible and cannot be proven.

 
### Install Steghide:
     
     sudo apt install steghide
  
 ![stegphide install](https://github.com/user-attachments/assets/e50d639a-6f1f-433e-8ae4-d0a81d911dd9)

Prepare the Files:
- Choose the image file you want to use (e.g., cover.jpg).

- Prepare the file you want to hide (e.g., secret.txt/ file.pdf/ audio.mp3).

### Embed the File Inside the Image:

     steghide embed -cf cover.jpg -ef secret.txt

![stegphide2](https://github.com/user-attachments/assets/253021f6-52b4-409a-b4c7-7e3beb3df6a2)

It will prompt you to set a passphrase. This secures the hidden data.

### Verify the Embedding (Optional):

- To check if data is embedded:

       steghide info cover.jpg

![stegphide3](https://github.com/user-attachments/assets/6bc3668b-d895-4ca5-9ecb-299fca86f493)

### Extract the Hidden File Later:

      steghide extract -sf cover.jpg

![steghide4](https://github.com/user-attachments/assets/4a47c99e-64dc-4c64-80e0-58f782a34e64)

Enter the passphrase to retrieve the hidden file.

### Result:

The file secret.txt will be extracted in the current directory.






