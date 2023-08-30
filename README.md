# MPCNNs-A-Novel-Matrix-Profile-based-CNNs-Approach-for-Sleep-Apnea-Classification
# Abstract
Sleep apnea (SA) is a significant respiratory condition that poses a major global health challenge. Accurate detection of sleep apnea episodes is crucial for prompt therapies and enhanced patient outcomes. Previous studies have investigated several machine and deep learning models in order to assess the efficacy of electrocardiogram (ECG)- based SA diagnoses. Despite these advancements, conventional feature extractions derived from electrocardiogram (ECG) signals, such as R-peaks and RR intervals, may fail to capture crucial information encompassed within the complete PQRST segments. In this study, we introduce a method that aims to bridge this diagnostic gap by delving deeper into the comprehensive segments of the ECG signal. Our approach was inspired by the distance information in Matrix Profile algorithms. The algorithms generate a Euclidean distance profile from a set of subsequences of fixed-length signals. From this, we derived the Min Distance Profile (MinDP), Max Distance Profile (MaxDP), and Mean Distance Profile (MeanDP) based on the minimum, maximum, and mean of the profile distances, respectively. To validate the performance, we employ the LeNet-5 architecture as the primary CNN model. To assess the robustness of this performance, we also conduct tests using two distinct lightweight models, namely BAFNet and SE-MSCNN. Our experimental results on the PhysioNet Apnea-ECG dataset revealed that with our novel feature extraction method, we achieved a per-segment accuracy up to 92.11 \% and a per-recording accuracy of 100\%, along with the highest correlation value of 0.989. By introducing a new feature extraction method based on distance relationships, we enhanced the performance of certain lightweight models, showing potential for home sleep apnea test (HSAT) and SA detection in IoT devices. 
![overall](https://github.com/sportsengineeringvn/MPCNNs-A-Novel-Matrix-Profile-based-CNNs-Approach-for-Sleep-Apnea-Classification/assets/104493696/77d50d20-048e-40ec-8878-8947d55451e6)
# Dataset
The data is available at https://physionet.org/content/apnea-ecg/1.0.0/
# Usage
1. Dowload the data from the above website.
2. Run the preprocessing file to get the file pkl (T1 is the highest performance). Please read the paper to understand abaout the design of T1,T2,T3 and T4.
3. Per-segment classfication: With the preprocessing data run with different architecture: LeNet-5_model.ipynb, SE-MSCNN_model.ipynb, BAFNET_model.ipynb.
4. Per-recording classification: After have the csv file in steps 3 run file test_per_recording.ipynb to got the result. The result display in Table3.csv
# Our performance setups
Run in Google Colab T4-GPU with High RAM, Python==3.10.12, Keras==2.12.0, and TensorFlow==2.12.0
# Email
If you have any question, please email to: 21hieu.nx@vinuni.edu.vn
