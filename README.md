Assuming that you already have a system for detecting handwriting using OCR, here the next task is given an input image that contains handwritten text, and an image we have to extract the image from the text.

# Image_Extraction
Here the code for extracting images from an image or a scanned book is attached.

flow of the code is:
1. Convert the image to grayscale, which is necessary for some of the algorithms
2. Apply a binary filter converting image to black and white
3. Optionally, apply an erode or dilate filter (Here dilation is used)
4. Optionally, apply Canny edge detection
5. Find contours (i.e. what appears to be lines)
6. Filter contours which are very small or very large, to avoid extracting small things like defects, letters, etc. or large artifacts like borders from the scanning process which span an entire edge


# Input
All the input files can be found in /content/sample_data/ folder in colab named as:
1. download.jpeg
2. images1.jpeg
3. images2.jpeg
4. Capture.png
5. urinary.jpeg

# Output
All the output files can be found in /content/sample_data/output folder in colab. Here some text containing images are also detected but this problem can be solved by adding a system for detecting handwriting using OCR.
