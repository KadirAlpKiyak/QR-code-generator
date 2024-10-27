# QR-code-generator
This Python code creates a graphical user interface (GUI) for generating QR codes using the Tkinter library for the interface and the qrcode library to create the QR codes. Here’s a breakdown of its main components and functionality:


Window Setup:

The main window (wn) is created using Tkinter, with a title and size. The background color is set to SteelBlue3.
Header Section:

A label at the top displays the title “Generate QR Code with DataFlair,” framed with a background for emphasis.
Input Fields:

The interface includes fields for user input:
Text/URL: The text or URL the user wants to encode in the QR code.
Save Location: The directory path where the QR code image will be saved.
Image Name: The desired name for the QR code image file.
Size: An integer input for the QR code version size (between 1 and 40), controlling the QR grid’s dimensions.
Generate Code Function:

The generateCode function reads the inputs, creates a QR code with the specified parameters, and saves it as an image file in the given directory.
The function utilizes the qrcode.QRCode class with user-defined size, box size, and border.
If successful, it shows a message box confirming the QR code has been saved; errors trigger an error message.
Generate Button:

A "Generate Code" button calls the generateCode function to create the QR code based on the provided inputs.
This code is ideal for users needing a quick tool to generate and save QR codes for URLs, text, or other information directly from a graphical interface.
