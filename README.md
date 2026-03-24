# knee-orthretis-severity-classification
Knee osteoarthritis causes joint damage, leading to pain and reduced mobility. Manually grading its severity from X-ray images is slow and error-prone. This project aims to use deep learning to automate the classification, ensuring faster and more accurate diagnosis.


obj:
  The objective is to develop a real-time system that uses deep learning to automatically classify the severity of knee osteoarthritis from X-ray images, enabling faster diagnosis and assisting doctors in making accurate treatment decisions.

Automate the classification of knee osteoarthritis severity using deep learning.
Improve diagnosis speed and accuracy by analyzing X-ray images.
Provide a web interface for real-time severity prediction.
Assist doctors in making better treatment decisions.

constraints:
  Data Imbalance: Uneven distribution of X-ray images across severity levels may affect model accuracy.
  Model Interpretability: Understanding and explaining predictions can be challenging.
  High Computational Demand: Training deep learning models requires significant processing power.
  Limited Dataset Quality: Variations in image quality can impact classification performance.
  Real-time Performance: Ensuring fast predictions while maintaining accuracy may be difficult.

methodolgy:
  1 Image Processing (OpenCV + NumPy)
  Resizing, Normalization, Data Augmentation
  2.Dataset Processing (Pandas + Scikit-learn)
Load and Split Dataset, Preprocessing 
  3.Deep Learning Model (TensorFlow/Keras)
Classifies Severity
  4.Grad-CAM for Explainability
Highlights Key Regions, show predictions


how to run:
shell
(base)$: git clone https://github.com/vasudevan31195-star/knee-orthretis-severity-classification/edit/main/README.md)
(base)$: cd knee_OA_dl_app

shell
    (base)$: conda env create -f environment.yml

conda activate knee_dl_app

Download `model_Xception_ft.hdf5` model from
   [here](https://drive.google.com/file/d/1vPS_j2AW3M1W8GydREEDw6CDENSgVwCy/view?usp=share_link)
   to run the application. Create `models` folder and copy the model here.


    (knee_dl_app)$: mkdir src/models

- Download the dataset from [Knee Osteoarthritis Dataset with Severity
   Grading](https://www.kaggle.com/datasets/shashwatwork/knee-osteoarthritis-dataset-with-severity)
   to train the model and test the application. Create `dataset` folder and copy
   the data here.

    
    (knee_dl_app)$: mkdir dataset
    

- Run it:

    (knee_dl_app)$: streamlit run app/app.py



