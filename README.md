# Alibaba Challenge

<b>This notebook contains 3 main sections:</b>

    1. Data Analysis
    2. Plain Ellipse Classification (only detects if the images contain ellipses or lines)
    3. Ellipse Parameters Classification (detects ellipse and their parameters in images)
    
<b>Those steps were done before running classification:</b>
    
    1. Analyzing data I found that for some reason train_data.txt and test_data.txt were not properly formatted. Fixed it.
    2. Ellipse are symmetrical objects thus:
        a. The ellipses rotated by angles such as 10 and 190 look the same. Fixed it by removing 180 degrees from angles greater than 180.
        b. The ellipses rotated by 90 degrees or with a swapped axis look the same. Fixed it by removing 90 degrees and swapping axis on angles greater than 90S
        
<b>Short Description:</b>

    The backbone of the notebook including data analysis, data preparation, models definition, training and metrics were completed in less than 3 hours. However, then I realized that angle accuracy was way below expected results. Thus, it took another few hours to understand why it happened (I had to align angles with the axis, see section above).
