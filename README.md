* **Parkinson Disease :** This dataset involves predicting whether a patients is  set to 0 for healthy<br> and 1 for PD(Parkison disease) :


# [Dataset]()
   *The dataset was created by Max Little of the University of Oxford, in 
collaboration with the National Centre for Voice and Speech, Denver, 
Colorado, who recorded the speech signals. The original study published the 
feature extraction methods for general voice disorders.*

  *Data Set Information:*

*This dataset is composed of a range of biomedical voice measurements from 
31 people, 23 with Parkinson's disease (PD). Each column in the table is a 
particular voice measure, and each row corresponds one of 195 voice 
recording from these individuals ("name" column). The main aim of the data 
is to discriminate healthy people from those with PD, according to "status" 
column which is set to 0 for healthy and 1 for PD.*

*The data is in ASCII CSV format. The rows of the CSV file contain an 
instance corresponding to one voice recording. There are around six 
recordings per patient, the name of the patient is identified in the first 
column.For further information or to pass on comments, please contact Max 
Little (littlem '@' robots.ox.ac.uk).*

*Further details are contained in the following reference -- if you use this 
dataset, please cite:
Max A. Little, Patrick E. McSharry, Eric J. Hunter, Lorraine O. Ramig (2008), 
'Suitability of dysphonia measurements for telemonitoring of Parkinson's disease', 
IEEE Transactions on Biomedical Engineering (to appear).*
*The data & attributes information for this project is available at<br> https://archive.ics.uci.edu/ml/machine-learning-databases/parkinsons/*




### [Attributes information:]()
   * *Matrix column entries (attributes):*
   * *name - ASCII subject name and recording number*
   * *MDVP:Fo(Hz) - Average vocal fundamental frequency*
   * *MDVP:Fhi(Hz) - Maximum vocal fundamental frequency*
   * *MDVP:Flo(Hz) - Minimum vocal fundamental frequency*
   * *MDVP:Jitter(%),MDVP:Jitter(Abs),MDVP:RAP,MDVP:PPQ,Jitter:DDP - Several *
   * *measures of variation in fundamental frequency*
   * *MDVP:Shimmer,MDVP:Shimmer(dB),Shimmer:APQ3,Shimmer:APQ5,MDVP:APQ,Shimmer:DDA - Several measures of variation in amplitude*
   * *NHR,HNR - Two measures of ratio of noise to tonal components in the voice*
   * *status - Health status of the subject (one) - Parkinson's, (zero) - healthy*
   * *RPDE,D2 - Two nonlinear dynamical complexity measures*
   * *DFA - Signal fractal scaling exponent*
   * *spread1,spread2,PPE - Three nonlinear measures of fundamental frequency variation* 
   

### [Experiment Results:]()
* **Data Analysis**
    * *All columns contain outliers except for N.*
 * **Performance Evaluation**
    * *Splitting the dataset by 80 % for training set and 20 % validation set.*
 * **Training and Validation**
    * *GausianNB gets a higher accuracy score than other classification models.*
    * *GaussianNB ( 99 % accuracy score )*
 * **Fine Tuning**
    * *Model : Extreme GradientBoosting Classifier*
    * *Best: 0.932143 using {'learning_rate': 0.1, 'max_depth': 3, 'n_estimators': 75*
 * **Performance Results**
    * *Training Score: 99.64%*
    * *Validation Score: 98.57%*
    * *accuracy score: 0.9857*
    * *roc auc score: 0.98*
    * *f1 score: 0.9795*
    * *precision score 1.0*
    * *recall score 0.96*

 classification_report :

              precision    recall  f1-score   support

         0.0       0.98      1.00      0.99        45
         1.0       1.00      0.96      0.98        25

                                       0.99        70
                   0.99      0.98      0.98        70
                   0.99      0.99      0.99        70







