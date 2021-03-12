# Spectrum Challange 2 Dataset and Frame Error Prediction Code
Deep Learning for Frame Error Prediction using a DARPA Spectrum Collaboration Challenge (SC2) Dataset.

# Code
The code is provided into separate files, one for each scrimmage. Every file contains five different neural network architectures, with two separate approaches for creating the train-validation-test set. Please refer to the paper for a detailed description.

# Dataset
The dataset is approved for public release, distribution unlimited.

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

Here are the links to the dataset files mentioned in the code (one pickle file for each scrimmage):

[Scrimmage 4](https://purdue0-my.sharepoint.com/:u:/g/personal/amahdeej_purdue_edu/EQsfaBF0MjJNvBXqkPq-Lv0BlyAm8ph8O85s-vxOqVjJTA?e=pYHIQS) (547.5 MB) [Mirror](https://app.box.com/s/i0c1qimr0mjuyr38celtxbsuedhlp9tr)

[Scrimmage 5](https://purdue0-my.sharepoint.com/:u:/g/personal/amahdeej_purdue_edu/EVnfh_V2BZBOk9SOTvKDLa4BGQ54LA9rr_r0cfFQWC_SLw?e=Jh4yCL) (979.7 MB) [Mirror](https://app.box.com/s/sqyvrapww6z5ydg0rrx7tjszs32bhndx)

A larger dataset containing the more information about each match is also available. Please refer to SC2_Dataset_Documentation.pdf for more details regarding the structure of the full dataset.

Here is the link to the full dataset (separate sqlite files for each match):

[Full Dataset](https://purdue0-my.sharepoint.com/:f:/g/personal/amahdeej_purdue_edu/EszW2WkpQWBLg9Y6cYX1FtUBpEyMS5XpUuCUxa2vFj5nXg?e=Nh0tk6) (136 GB) [Mirror (Needs Access Request)](https://app.box.com/s/snwqgmzxljjsu129wampesj0xgn2ozpq)

