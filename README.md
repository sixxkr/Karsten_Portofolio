# Karsten Errando Winoto Portofolio

# [Project 1 : Heart Guard](https://github.com/sixxkr/heartguard)

This is a project I did for my Mobile Application Programming course at university, where I built a classification model for heart disease that was implemented into a mobile application.

- Data was taken from Kaggle (https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset)
- The Model using Random forest
- For making this mobile app, I using flutter framework
- I using local API To Integrate mobile app with model machine learning using flask

## Mobile App Layout

![HeartGuard_1](https://github.com/user-attachments/assets/d5257e73-684d-4cba-9f3a-e3272b8e6725)&nbsp; &nbsp; &nbsp;
![HeartGuard_2](https://github.com/user-attachments/assets/60a580ff-6144-4d01-b42f-35734caa9fe9)

## Model Accuracy

![HeartGuard_1](Images/HeartGuard_3.PNG)

# [Project 2 : Transformer Leopard Gecko ](https://github.com/sixxkr/Transformer_Leopard-Gecko)

This is a project I did for my Pattern Recognition course at university, for my final project in this class.

- This model classifies images of Leopard Geckos into 3 morph categories:
  - `Boldstripe`
  - `Albino`
  - `Albino Boldstripe`
- Dataset consists of ~60 images collected manually from the internet. Data was taken from google, instagram, etcera.
- The model is built using a Transformer architecture.
- Dataset is split into training and testing sets.
- The model is trained for 100 epochs.
- Achieved testing accuracy: **41%**

## 🗂️ Dataset

- ✅ Total Images: ~60
- ✅ Classes:

  - **Boldstripe** :

    ![Boldstripe](Images/DS_GEKCO/BOLDSTRIPE/4.jpg)

  - **Albino** :

    ![Boldstripe](Images/DS_GEKCO/ALBINO/11.jpg)

  - **Albino Boldstripe** :

    ![Boldstripe](Images/DS_GEKCO/BOLDSTIPE_ALBINO/3.jpg)

## 🧪 Evaluation Results

- **Test Accuracy**:

  ![test](Images/hasil_testing.png)

- **Train Accuracy and Loss**:

  ![test](Images/Training.png)

# [Project 3 : App_Koperasi ](https://github.com/sixxkr/app_koperasi)

This is a mobile cooperative (koperasi) application I built during my internship at **Dua Kelinci**.  
It helps factory employees browse products, add items to cart, check out, and track their transaction history.

- Built with:
  - **Flutter** for the mobile frontend (Android/iOS).
  - **Flask** + **MySQL** for the backend API and database.
- Core features:
  - View product catalog with details.
  - Add to cart, update quantities, remove items.
  - Checkout flow (order summary, payment placeholder/integration-ready).
  - Transaction history with order status.
  - User authentication (login/logout) and session handling.
- Architecture:
  - RESTful API built in Flask.
  - Persistent storage in MySQL.
  - Frontend–backend communication via JSON over HTTPS.

# Project 4 : ECG Heart Disease Classification with Deep Learning

This is a project I did for my Final Thesis at university, where I built a classification model for heart disease based on ECG signal amplitude using several deep learning methods.

## Data

Data was taken from Kaggle (https://www.kaggle.com/datasets/shayanfazeli/heartbeat)

![Dataset](Images/ecg_heartbeat_categorization%20Dataset.png)

## The models used are 4 types of deep learning architectures:

- CNN1D (Convolutional Neural Network)

- RNN (Recurrent Neural Network)

- LSTM (Long Short-Term Memory)

- GRU (Gated Recurrent Unit)

## Model structure was designed :

- **CNN1D** :
  ![CNN1D](Images/arsitektur%20cnn.svg)
- **RNN** :

  ![RNN](Images/rnn.png)

- **LSTM** :

  ![LSTM](Images/LSTM.png)

- **GRU** :

  ![GRU](Images/GRU.png)

## Exploratory Data Analysis (EDA)

The dataset used in this project was taken from Kaggle and consists of two parts: training dataset and testing dataset.

- Training set : 87,554 samples

- Testing set : 21,892 samples

- Each ECG signal has a duration of 1870 ms with a frequency of 120 Hz.

### Class Distribution (before preprocessing)

| Class                             | Training   | Testing    |
| --------------------------------- | ---------- | ---------- |
| Normal                            | 72,471     | 18,118     |
| Fusion of paced and normal        | 6,431      | 1,608      |
| Premature ventricular contraction | 5,788      | 1,448      |
| Atrial Premature                  | 2,223      | 556        |
| Fusion of ventricular and normal  | 641        | 162        |
| **Total**                         | **87,554** | **21,892** |

## Preprocessing

Several preprocessing steps were applied before training:

- Label Encoding

  - Normal = 0

  - Atrial Premature = 1

  - Premature ventricular contraction = 2

  - Fusion of ventricular and normal = 3

  - Fusion of paced and normal = 4

- Data Splitting

  - Training set → split into 80% training and 20% validation

  - Testing set → used as provided

### Class Distribution (after splitting)

| Class                             | Training   | Validation | Testing    |
| --------------------------------- | ---------- | ---------- | ---------- |
| Normal                            | 57,892     | 14,579     | 18,118     |
| Fusion of paced and normal        | 5,182      | 1,249      | 1,608      |
| Premature ventricular contraction | 4,676      | 1,112      | 1,448      |
| Atrial Premature                  | 1,797      | 426        | 556        |
| Fusion of ventricular and normal  | 496        | 145        | 162        |
| **Total**                         | **70,043** | **17,511** | **21,892** |

### Example visualization of heartbeat signals:

- **Normal** :
  ![Normal](Images/0.svg)
- **Atrial Premature** :
  ![Atrial Premature](Images/1.svg)
- **Premature ventricular contraction** :
  ![Premature ventricular contraction](Images/2.svg)
- **Fusion of ventricular and normal** :
  ![Fusion of ventricular and normal](Images/3.svg)
- **Fusion of paced and normal** :
  ![Fusion of paced and normal](Images/4.svg)

## Model Evaluation

The results are shown in the following figures :

### Training

- **CNN**
  ![CNN](Images/cnn1d_1/train_val%20Loss.png)
- **RNN**
  ![RNN](Images/RNN1/train%20val%20loss.svg)
- **LSTM**
  ![LSTM](Images/lstm1/train%20loss_val.svg)
- **GRU**
  ![GRU](Images/GRU1/train%20val%20loss.svg)

### Testing

- **CNN**

  ![CNN](Images/cnn1d_1/cm.svg)

- **RNN**

  ![RNN](Images/RNN1/cm.svg)

- **LSTM**

  ![LSTM](Images/lstm1/cm.svg)

- **GRU**

  ![GRU](Images/GRU1/cm.svg)

### Results

The evaluation results of each model using the test dataset are summarized below:

| Model | Accuracy | Precision | Recall | F1-Score |
| ----- | -------- | --------- | ------ | -------- |
| CNN   | 0.98     | 0.92      | 0.90   | 0.91     |
| RNN   | 0.83     | 0.17      | 0.20   | 0.18     |
| LSTM  | 0.97     | 0.89      | 0.79   | 0.82     |
| GRU   | 0.98     | 0.90      | 0.89   | 0.90     |
