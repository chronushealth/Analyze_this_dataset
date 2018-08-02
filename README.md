# Analyze this dataset

# Problem 1 : Tell me more about this data set
Take a look at two time series data files, the data set is a single column data set 
* signal_1.dat
* signal_2.dat

## Information about the dataset
* signal_1.dat is a measured signal for 1s. Data is sampled at Fs = 50kHz. Records multiple events. 
* signal_2.dat is a single pulse giving characteristic information about an event occuring. 
* Both signals are electrical measurements

For both datasets, height, width and area under the pulse give us characteristic information about the event. 

## Task and questions
* Use signal_1 to learn more about the event. What are you inferences
* Signal_2 is a ideal single pulse. Using signal_2, what can you infer about signal_1
* Can you infer anything about the noise characteristics

## Time required
1 - 2 hrs (Typical 1 hr)

# Problem 2: Exploratory data set

## Dataset
* Download the dataset from https://drive.google.com/drive/folders/18ptQRTf85MOJbgRYhQYd_oK0WdoVJNPI?usp=sharing
* The dataset is in binary format
* Both datasets are electrical measurements with sampling rate Fs = 250MHz
* To convert dataset, here is one way to do it
```python
import numpy as np

inputSignal = np.fromfile(file='CHA.bin', dtype=np.int16)
outputSignal = np.fromfile(file='CHB.bin', dtype=np.int16)
```
* Variations in signal intensity indicate events. Inferences are similar to Dataset 1, so amplitude of variation, width and area give characteristic information.

## Task and questions
* Tell us more about the relationships between the input and output. 

## Time
Limit working on this dataset to 30 mins. 



