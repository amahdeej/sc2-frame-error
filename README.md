# ssp2020sc2
Spectrum Challange 2 Dataset and Frame Error Prediction Code

# Dataset
The dataset is contained in two files - scrimmage4_link_dataset.pickle and scrimmage5_link_dataset.pickle

The pickle files are stored as list of tuples, each list corresponding to a single link, and containing two elements. Each element a length equal to the number of frames in that link - it varies between link to link.
The first tuple is contains the paramenters -
1. Signal to Noise Ratio ('snr') - 1 element
2. The Modulation and Coding Scheme ('mcs') - 1 element
3. The center frequency of the link ('centerFreq') - 1 element
4. The bandwidth of the link ('bandwidth') - 1 element
5. The Power Spectral Density ('psd') - 16 elements
Thus the total width of each element of the first tuple for a link is 20.

The second tuple contains the success of transmission ('rxSuccess'). If it is 1, there is no frame error, if it is 0, ther is a frame error.

# Code
The code is provided into separate files, one each for a specific simulation. Every file contains two training approaches - regular training and bagging. Please refer to the paper for a detailed description.

# Alternate Download Links
If the dataset files can not be downloaded due to bandwidth limit of github being crossed, here are links for them from onedrive:

[Scrimmage 4](https://purdue0-my.sharepoint.com/:u:/g/personal/amahdeej_purdue_edu/EQsfaBF0MjJNvBXqkPq-Lv0BlyAm8ph8O85s-vxOqVjJTA?e=EiSxIq)
[Scrimmage 5](https://purdue0-my.sharepoint.com/:u:/g/personal/amahdeej_purdue_edu/EVnfh_V2BZBOk9SOTvKDLa4BGQ54LA9rr_r0cfFQWC_SLw?e=EJ5nWr)
