# Spectrum Challange 2 Dataset and Frame Error Prediction Code
Deep Learning for Frame Error Prediction using a DARPA Spectrum Collaboration Challenge (SC2) Dataset.

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
The code is provided into separate files, one for each scrimmage. Every file contains five different neural network architectures, with two separate approaches for creating the train-validation-test set. Please refer to the paper for a detailed description.

# Dataset
The dataset is approved for public release, distribution unlimited.

Details about the dataset are mentioned in SC2_Dataset_Documentation.pdf

Here are the links to the dataset files mentioned in the code:

[Scrimmage 4](https://app.box.com/s/i0c1qimr0mjuyr38celtxbsuedhlp9tr)

[Scrimmage 5](https://app.box.com/s/sqyvrapww6z5ydg0rrx7tjszs32bhndx)


