# N.R.E.AL 
## Noise Removal Algorithm



Noise Reduction using Minimum Mean Square Estimators (MMSE) can be used where the enhancement of noisy speech signals is essentially an estimation problem in which the clean signal is estimated from a given sample function of the noisy signal. The goal is to minimise the expected value of some distortion measure between the clean and estimated signals.

Methodology :
1.First, we read the voice sample in terms of integral values of displacement from the mean position in the audio signal, as a numpy array.

2.After reading the audio file as the required data , we apply minimum mean squared estimation on the data extracted .

3. Applying Spectral Gating Noise Reduction. Through spectral gating we can get rid of the rest of the residual noise points.Noise Gate is like a device that helps us control the volume of the audio signal, which is represented by the amplitude of the audio signal. So passing the audio signal through the spectral gate, we intentionally bring down the volume of the suspected noise signals.

4. We can try re-enhancing the audio signal by applying the M.M.S.E. enhancement once again in order to slightly strengthen the resultant signal. This is not a required process but it does help in subtly strengthening the audio signal.

RESULTS :

Initial input : 
![image](https://user-images.githubusercontent.com/81297719/112599165-90e0e200-8e35-11eb-972a-be4d61058278.png)

AUDIO SAMPLE : https://user-images.githubusercontent.com/81297719/112599467-f9c85a00-8e35-11eb-8a02-c8cd10afc43e.mp4


After LOGMMSE:|
![image](https://user-images.githubusercontent.com/81297719/112599557-1e243680-8e36-11eb-80d9-0493884efce5.png)

After Sperctral Gating :|
![image](https://user-images.githubusercontent.com/81297719/112599596-2e3c1600-8e36-11eb-927e-420de9ba6432.png)

Re-enhancement:|
![image](https://user-images.githubusercontent.com/81297719/112599704-4ca21180-8e36-11eb-8670-2a88183c8128.png)

AUDIO SAMPLE (CLEANSED): https://user-images.githubusercontent.com/81297719/112599985-9d196f00-8e36-11eb-9116-0be0c1549f92.mp4



