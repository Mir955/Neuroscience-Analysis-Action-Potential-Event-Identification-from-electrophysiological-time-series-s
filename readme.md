# Neuroscience Analysis: Action Potential Event Identification from electrophysiological time series signal

The extracellular recording of neural signals consists of action potentials from several neurons. The information of the nervous system is encoded in the form of firing frequency or firing time, the first procedure in the interpretation of neuronal signals is the detection of the action potential firing, i.e., the neural spike.

![](Images/signal1.png=150x50)

Since the proposed action potential detector does not require a quantitative knowledge of the signal and noise of the recording under investigation, it can be utilized for the online or first offline analysis of neural signal recordings, where such quantitative information is not readily available.

# Method_1: 
Mathematics computation of action potential detection. In method 1, a threshold at 0-20 mv is set. Thus, intercept to this threshold line is measured using three methodology, 1. Rising (Depolarisation) 2. Falling (Repolarisation) 3. Both.

# Method_2: 
In this method, CWT transform to the whole time-series signal is applied to compute elicite (action potential) events index. Full form of CWT is Continuous Wavelet Tranform. In CWT, a time-series signal is multiplied with mother wavelet function signal and 1-D time series signal is converted into 2D images (stored in CWT_Image folder created). An carefull observation of dataset, that a full action potential event takes in total 610 samples (repetative pattern). 

# Dataset: 
#Few Observations about the dataset:
![](Images/signal.png=150x50)

* As the sampling frequency is 50KHz. We can see that each sample is acquired at a gap of 0.02 ms.
* The whole data is recorded for a time-span of 1.2 s (approx).
* Depolarizing step is started from 200ms and ended at 1000ms.
* We can see that the a single action Potential rises from -65mV and reaches a peak of 45mV(approx) and comes bact to -65mV
* This cycle took 600 samples of reading i.e. 350*0.02ms = 7 ms 

In total 63 action potential events have occured in this 1.2 secs of data. 