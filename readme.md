# Master-level tutorial on WSET-CNN-BKA-LSSVM diagnosis, bearing and gearbox fault diagnosis at Southeast University, MATLAB code, highly recommended!

The theme of this article is:
Propose a WSET-CNN-BKA-LSSVM method for fault diagnosis. The method includes:
1. Firstly, utilize wavelet synchronization extraction transformation (WSET) to extract the time-frequency resolution of the collected fault data, perform mode decomposition and processing on the extracted data, obtain the decomposed time-frequency image, and reduce the dimensionality of the image;
2. Input the time-frequency image obtained in the first step into a two-dimensional convolutional neural network (CNN) for adaptive fault feature extraction;
3. Take the output of the fully connected layer as the input for the least squares support vector machine (LSSVM), and use the new algorithm of 2024 SCI Category I: Black-winged eagle optimization algorithm to optimize the two key parameters of LSSVM.
4. This tweet based on experiments with bearing data and gearbox data from Southeast University. The experiments show that even with only 30 experimental samples, the method can achieve more than 98% accuracy. This fully demonstrates the applicability of the method in fault diagnosis with small sample sizes.
Detailed explanation:
Data Processing:
① Perform a brief processing and labeling of the official downloaded bearing data and gearbox data from Southeast University, as follows:
Bearing data selected are as follows:
'ball 20_0.csv': Rolling element failure
'comb_20_0.csv': Composite failure
'health_20_0.csv': Healthy
'inner_20_0.csv': Inner ring failure
'outer_20_0.csv': Outer ring failure
Extract the third column of these five data files, integrate them into a data_total.mat file, which contains 5 types of fault types, totaling 1000 samples. Set each type of sample to 200, each sample has 2048 points, using sliding windows of size 2048 and a sliding step of 1000. The process for gearbox data is similar to that of bearing data, so it will not be elaborated upon further. The program includes code explanations.
2. Implementation Details
- Use Wavelet Synchronous Extraction Transform (WSET) to convert data into time-frequency diagrams.
- Feed the constructed feature vectors into different models for training and testing.

Results Display:
Dongdang University Bearing Fault Diagnosis Results:
- For each state, use the first 120 groups for training and the last 80 groups for testing. The results are as follows:
- Classification results using WSET-CNN-BKA-LSSVM, along with t-SNE dimensionality reduction distribution before and after CNN model recognition:
- It can be seen that the precision rate of the proposed method reaches 100%.

To verify the advantages of the proposed model in small sample bearing fault diagnosis, use the first 30 groups for training and the last 170 groups for testing. The results are as follows:
- Precision rates can reach 99.0588% under the condition of small sample fault diagnosis, which sufficiently demonstrates the advantages of this study in small sample fault diagnosis!

Dongdang University Gearbox Fault Diagnosis Results:
- For each state, use the first 120 groups for training and the last 80 groups for testing. The results are as follows:
- Classification results using WSET-CNN-BKA-LSSVM, along with t-SNE dimensionality reduction distribution before and after CNN model recognition:
- It can be seen that the precision rate on gearbox data reaches 99.25%.
- To verify the advantages of the proposed model in small sample gearbox fault diagnosis, use the first 30 groups for training and the last 170 groups for testing. The results are as follows:
- Precision rates can reach 95.1765% under the condition of small sample fault diagnosis, which sufficiently demonstrates the advantages of this study in small sample fault diagnosis!

All images can be run out.
Code Directory:
Divided into Dongdang University bearing diagnosis and gearbox diagnosis.
The code is very well organized! Ensure that beginners can understand it step by step, with detailed explanations in each section.

## Images

<!-- PAYMENT_BLOCK -->

## Get this dataset

- Payment link (Stripe): [Buy now](https://buy.stripe.com/3cs8yP7sY87d0vu9AB)
- Payment QR code: ![Payment QR code](pay.png)

<!-- /PAYMENT_BLOCK -->
