# Face Recognition Setup with Dlib and NumPy

## Overview

This document provides information on the setup and dependencies required to run a face recognition system using Dlib and NumPy on Python 3.9.13. It also includes a common error encountered and its solution.

## Python Version

Ensure you are using **Python 3.9.13** for compatibility.

## Issue Faced

When running the face recognition system, the following error was encountered:

```
RuntimeError: Unsupported image type, must be 8bit gray or RGB image.
```

### Solution

The error occurs due to an incompatible NumPy version. The issue was resolved by **downgrading NumPy to version 1.26.4**.

```sh
pip uninstall numpy
pip install numpy==1.26.4
```

After performing the downgrade, the face recognition system worked correctly.

## Not working then contact i'll help you for this 
<h4 align="center"> 📩 Get in touch: </h4>

```sh
ankitsharma7805@gmail.com
```

## Additional Notes

- Make sure that **Dlib is properly installed** with CMake support.
- If issues persist, verify the image format being passed to Dlib. It must be in **8-bit grayscale or RGB format**.
- Use `cv2.cvtColor(image, cv2.COLOR_BGR2RGB)` if required to convert the image to the correct format.

## Conclusion

This README serves as a reference for setting up a working environment for face recognition using Dlib. Keeping dependencies at compatible versions ensures smooth execution without errors.

