# Face Recognition

This code is a simple implementation of face recognition using the `face_recognition` library in Python. It allows you to identify and label faces in an image.

## Prerequisites
- Python 3.x
- `face_recognition` library
- `opencv-python` library

## Installation
To install the required libraries, use the following commands:
```
pip install face_recognition
pip install opencv-python
```


## Usage
1. **Prepare the face images**: 
   - Create a folder named "faces".
   - Place the images of the faces you want to recognize in the "faces" folder. The images should be in JPG or PNG format.
   - Each image should contain only one face.

2. **Encode the faces**:
   - Run the `get_encoded_faces()` function to encode the faces in the "faces" folder. This function returns a dictionary with the face names as keys and the corresponding encodings as values.

3. **Recognize faces in an image**:
   - Call the `classify_face(im)` function and pass the file path of the image as the `im` parameter.
   - The function will load the image, detect faces, and compare them with the known faces.
   - If a match is found, the face will be labeled with the corresponding name.
   - The function returns a list of recognized face names.

4. **Display the image**:
   - The code includes a loop that continuously displays the image with the recognized faces boxed and labeled.
   - Press 'q' to exit the loop and close the image window.

Example usage:
```python
print(classify_face("test.jpg"))
```

# Notes

The code assumes that the face images are stored in a folder named "faces" in the same directory as the script.
The face_recognition library uses deep learning models to encode and compare faces, which requires significant computational resources.
The code may not perform well in certain lighting conditions, with low-resolution images, or with faces that are partially covered or at unusual angles.
Please ensure you have the necessary permissions and rights to use the images and comply with applicable privacy and data protection regulations.

# Credits

This code utilizes the face_recognition library, developed by Adam Geitgey. For more information about the library and its usage, refer to the official documentation: https://github.com/ageitgey/face_recognition
