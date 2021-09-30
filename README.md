# Steel-Plate-Fault-Diagnosis



## Objective:

   The objective of the project is to classify steel plates fault into 7 different types. The end goal is to train several machine Learning Algorithms for automatic pattern recognition. In doing so, I have employed **Logistic Regression**, **KNN**, **Naïve Bayes**, **Decision Trees** and **Random Forest**. Also, I have used **_Cross-validation_** to find the most optimum hyper-parameters. Finally, I compare the models and see  how well each model perform using Classification metrics: Confusion Matrix, Precision, Recall and F-1 Score.

## Motivation:

A fault may be defined as an unacceptable difference of at least one characteristic property or attribute of a system from acceptable usual typical performance. The main purpose of any fault diagnosis system is to determine the location and occurrence time of possible faults on the basis of accessible data and knowledge about the performance of diagnosed processes. Manual fault diagnosis system is the traditional way where an expert with electronic meter tries to obtain some information about relevant operational equipment, check the maintenance manual and then diagnose the probable causes of a particular fault.  However, intelligent fault diagnosis techniques can provide quick and correct systems that help to keep product quality problems at bay and facilitates precautionary maintenance.    

        

This project evaluates the performances of several popular and effective data mining models to diagnose seven commonly occurring faults of the steel plate namely; Pastry, Z_Scratch, K_Scatch, Stains, Dirtiness, Bumps and Other_Faults.

 

## Data Collection:

URL : [http://archive.ics.uci.edu/ml/datasets/steel%2Bplates%2Bfaults]

### Source:

> Semeion, Research Center of Sciences of Communication, Via Sersale 117, 00128, Rome, Italy. 

www.semeion.it

### References:

>> M Buscema, S Terzi, W Tastle, A New Meta-Classifier,in NAFIPS 2010, Toronto (CANADA),26-28 July 2010, 978-1-4244-7858-6/10 Â©2010 IEEE

>> M Buscema, MetaNet: The Theory of Independent Judges, in Substance Use & Misuse, 33(2), 439-461,1998

## Workflow :

   1. **Exploratory Data Analysis**

       - 1.1 Count Plot to show the number of defects belonging to each defect type.

       - 1.2 Visual analysis of the correlation between the factors.

       - 1.3 Correlation Matrix    

       

   2. **Model Development and Classification**

        - 2.1 Data Preparation

        - 2.2 Model Development

            - 2.2.1 Logistic Regression

            - 2.2.2 SVM

            - 2.2.3 Random Forest

            - 2.2.4 Xg boost





  

    

     

            

    

  



      

     

      

          



   

## Results:

   1. EDA helps in giving a preliminary glimpse on how various factors are affecting the development of Defects.

       - We notice that 'other defects', 'bumps' and 'K_Scratch' are major defects.

   2. Cross-Validation is an effective way to find the best Hyper-parameters.

   3. Decision Tree outperforms other Non-Ensamble models.

 

   4. Random Forests can substantially increase the efficiency but are computationally expansive when dealing with a large dataset as in this case.

   

   

|    **Model**     |    **ROC AUC Score**    | **F1 Score**   |

 |:------------:|:-----------------------------:|:----------------------:|

 | `Logistic Regression`| 0.884 |0.60|

 | `SVM` | NAN |0.690|

 | `Xg boost `| 0.953 |**0.751**|



 | `Random Forest` | **0.933** |0.732|

 

 

 | **Model GridSearch CV**| **ROC AUC Score** | **F1 Score**|

 |:-----:| :-----------------------------: | :-------------:|

 | `Logistic Regression`|0.896 |0.636|

 | `SVM` | **NAN** |0.708|

 | `Xg boost` | 0.954 |0.774|



 | `Random Forest` | 0.953 |0.745|

## Conclusion:

Bagging and Boosting alogorithm performed well amongst the lot but still there is a margin to improve the performance.

Finally, I can say that this project was quite challenging as working on a multiclass classification problem containing 7 unique classes with imbalanced sets made it tough.

The model tuning and researching on parameters by understanding their use was the key highlight of this project.

    
