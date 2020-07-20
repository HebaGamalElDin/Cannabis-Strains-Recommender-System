# Cannabis-Strains-Recommender-System
This Project Is composed of Two main Parts ::

    1) Adding Medical_usage Column to the original Dataset found here From Kaggle :: 
               https://www.kaggle.com/kingburrito666/cannabis-strains
    
          => Hand Labeling for 400 Rows.
          => Using Description Column to Classify the Rest of "Medical_usage" Column (i.e Wheather Medical or Nonmedical Strain".
          
    2) Building a Recommender System using TFIDF, and Cosine Similarity (Linear_kernel)
    
    
    => Try Running The Notebook ::
        
        1) Check Requirments.txt File, Install all required packages, Download Pre-trained "Glove" Embeddings from Kaggle.
        2) Clone The Repository and let The "Cannabis_Orginal" Dataset Into The Same folder as the Notebook.
        3) Paste "glove.6B.50d.txt" file into the same folder as the Notebook.
        4) Run "Strain Recommender System_.ipynb" Notebook cell-by-cell.
     
    => Medical_usage Classification Model Accuracy and F1-Score ::
   
          1) Training Accuracy :: 100%
          2) Testing Accuracy :: 93%
          3) F1-Score :: (94% for "Non-Medical" Class) and (93% for "Medical" Class)
          
    
    => It was Challenging Working on only 400 Raws dataset.
   
     => Issues are met & its Solutions ::
   
        1) Class Imbalancing :: Resampling Technique Applied.
        4) Non-Linear Seperable Dataset :: 
           Ignoring simple linear ML models tried (SVM) and trying Kernal SVM then RNN with "Relu" Activation Function.
        3) RNN Vanashing :: Training with RNN-GRU Model.
        4) Overfitting caused by Resampling Technique :: l1_l2 Regularization Technique (Kernel, Bias) are Applied.
        
   **All Tries to Leverage The Testing Accuracy are so Welcomed.**
        
