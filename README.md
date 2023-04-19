# Can Detection and Classification Program

This program uses MATLAB to perform image processing on a set of pictures to detect and classify cans as either open or closed. The program reads in a series of image files, applies various image processing techniques, and then determines whether each can is open or closed based on its Euler number.

## More details about image processing program

The program reads in the image and, if it is not in grayscale, converts it to grayscale. Then, a binarization threshold is applied to distinguish the cans from the background. The resulting image is subjected to morphological operations, such as closing small gaps and canceling noise using the imclose function. Next, the bwlabel function is used to identify objects, followed by the regionprops function to compute various properties of each object, such as the Euler number, centroid, major and minor axis lengths, diameter, and radius. Based on these measurements, the program can determine whether a can is open or closed by examining its Euler number. The program also calculates invariant shape coefficients to help determine whether a can is open or closed. Finally, the viscircles function is used to draw circles around the cans and color them red or green, depending on whether they are open or closed. The program keeps track of the number of open and closed cans detected for each image using the count_o and count_z variables.

## Requirements
To run this program, you will need:

MATLAB R2019a or later
Image Processing Toolbox

## Usage
To use the program, follow these steps:

Open MATLAB and navigate to the directory where you cloned the repository.
Edit the p variable in the code to the number of pictures you want to analyze.
Place the pictures you want to analyze in the same directory as the program.
Run the program by typing can_detection in the MATLAB command window.
The program will generate a series of output images and display the number of open and closed cans detected in each picture.

## License
This program is licensed under the MIT License. See the LICENSE file for details.

## Author
This program was written by Justyna Neblik.
