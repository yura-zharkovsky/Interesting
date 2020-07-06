# Alibaba Challenge

This notebook contains 3 main sections:

1. Data Analysis
2. Plain Ellipse Classification (only detects if the images conatain ellipses or lines)
3. Ellipse Parametrs Classification (detects ellipse and their parameters in images)

Those steps were done before running classfication:
1. Analyzing data I found that for some reason train_data.txt and test_data.txt were not propely formated. Fixed it.
2. Ellipse are symetrical objects thus:<br> 
    a. ellipses rotated by angles such as 10 and 190 look the same. Fixed it by removing 180 degrees from angles greater than 180.<br>
    b. ellipses roatated by 90 degrees or with swapped axis looks same. Fixed it by removing 90 degrees and swapping axis on angles greater than 90
