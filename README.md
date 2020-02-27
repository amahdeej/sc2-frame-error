# ssp2020sc2
Spectrum Challange 2 Dataset and Frame Error Prediction Code

The dataset is contained in two files - scrimmage4_link_dataset.pickle and scrimmage5_link_dataset.pickle

The pickle files are stored as list of tuples, each list corresponding to a single link, and containing two elements. Each element a length equal to the number of frames in that link - it varies between link to link.
The first tuple is contains the paramenters -
1. Signal to Noise Ratio ('snr') - Length 1
2. The Modulation and Coding Scheme ('mcs') - Length 1 
3. The center frequency of the link ('centerFreq') - Length 1
4. The bandwidth of the link ('bandwidth') - Length 1
5. The Power Spectral Density ('psd') - Length 16
Thus the total width of each element of the first tuple for a link is 20.

The second tuple contains the success of transmission ('rxSuccess'). If it is 1, there is no frame error, if it is 0, ther is a frame error.

The code is provided into separate files, one each for a specific simulation. Please refer to the paper for a description of the methods.
