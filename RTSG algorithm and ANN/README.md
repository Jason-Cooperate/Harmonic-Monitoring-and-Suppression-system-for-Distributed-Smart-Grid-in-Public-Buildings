# Smart grid monitoring based on RTSG algorithm and Artificial Neural Network
 In this folder，we introduce RTSG algorithm and PQD classification based on deep learning.
## 1.RTSG
RTSG ,short for Real Time Synchronized Goertzel,is an advanced Goertzel algorithm proposed by our team.The RTSG consist of 2 phase：RTSAL interation for smart filtering & Interpolation Goertzel.
### 1) RTSAL
RTSAL is based on the signal segmentation algorithm after the marking process, and uses the MCT vectors to record the signal waveform over a specific period. RTSAL uses less sample data to compute and store waveforms by extracting information from important samples instead of all samples<sup>[1]</sup>. The RTSAL algorithm consists of two important parts: Segmentation and Labeling.
#### a)segmentation
By looking at the signal in Figure 3, a person can learn the characteristics of the signal. The signal may be interpreted as “noisy” in the beginning. Then it reaches a maximum and a minimum and grows and falls rapidly with a spike-like shape. After that, it starts to increase and then tends toward a stable value. The observers are aware of the signal behavior since they relate shape at different instants. Therefore, it is desirable to have a more complete sampling process in order to take into account sample sequences. The key process is to identify what the signal trajectory between samples is. It is not necessary to do this for every pair of samples. Therefore, the first process is to segment the signal and then relate these segments<sup>[2]</sup>.      
#### b)Labeling
Each time the difference is computed in the interpolation process, the sign of the error is recorded. When the segment ends, based on the majority of accumulated error signs, the behavior inside the segment can be classified. The error sign is the clue to classify the segment. If the signal is oversampled, the trajectory of the real signal inside the segment is restricted by the interpolation error<sup>[2]</sup>.The signal in each segment can be classified to 8 types('a','b','c','d','e','f''g','h'),each stands for a signal shape.
#### c) RTSAL process diagram
![RTSAL]()

### 2) RTSAL Interation for smart filtering

### 3) Interpolation Goertzel
