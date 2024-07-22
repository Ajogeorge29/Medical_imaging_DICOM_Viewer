DICOM Viewer and Converter
Overview
This repository contains a Python script designed for viewing and converting DICOM (Digital Imaging and Communications in Medicine) files. DICOM is the standard format for medical imaging data, and this script provides a simple and efficient way to visualize these images and convert them into more commonly used formats like PNG and JPEG.

Features
DICOM Image Viewer: Visualize DICOM images using the matplotlib library.
Image Conversion: Convert DICOM images to PNG and JPEG formats using the PIL (Pillow) library.
Normalization: Normalize the pixel values of DICOM images to enhance visualization and ensure compatibility with other image formats.
Dependencies
pydicom: For reading DICOM files.
matplotlib: For displaying DICOM images.
Pillow: For converting DICOM images to other formats.
numpy: For numerical operations and normalization of image data.
Installation
Before running the script, ensure you have the required Python libraries installed. You can install them using pip:

bash
Copy code
pip install pydicom matplotlib pillow numpy
Usage
View a DICOM Image:

Modify the dicom_file variable in the script to point to your DICOM file path and run the script to view the image.

python
Copy code
dicom_file = r"D:\2024\Medical_Imaging_Projects\0002.dcm"
view_dicom(dicom_file)
Convert DICOM Image to PNG and JPEG:

The script can also convert the DICOM file to PNG and JPEG formats. The output files will be saved in the same directory as the original DICOM file.

python
Copy code
convert_dicom(dicom_file, output_format='png')
convert_dicom(dicom_file, output_format='jpeg')
