# Credit_Risk_Analysis

## Overview
For this analysis, we are using machine learning models to predict credit risk.

## Results

### Random Oversampling Model
![image](https://user-images.githubusercontent.com/96644316/178440381-3900ec7c-b5b0-4858-8001-17cbe436dfd6.png)  
![image](https://user-images.githubusercontent.com/96644316/178440310-a188ebd2-fb0d-4f5b-b3dd-a05ddb3f8b59.png)  
![image](https://user-images.githubusercontent.com/96644316/178440107-fe650132-e93e-42a6-85da-daa7e3099a7a.png)  
* The balanced accuracy score is 65%.
* The high_risk precision is about 1% only with 62% sensitivity which makes a F1 of 2% only.
* Due to the high number of the low risk population, its precision is almost 100% with a sensitivity of 68%.

### Smote (Oversampling) Model
![image](https://user-images.githubusercontent.com/96644316/178440668-988bdc17-ddd8-4dd0-89c0-2a22c001070c.png)  
![image](https://user-images.githubusercontent.com/96644316/178440695-f33c1873-c783-4dc8-aad0-c3290b896161.png)  
![image](https://user-images.githubusercontent.com/96644316/178440721-d9fd2ae4-8451-4b1d-b2dc-d106f36c7848.png)  
* The balanced accuracy score is 64%.
* The high_risk precision is about 1% only with 63% sensitivity which makes a F1 of 2% only.
* Due to the high number of the low risk population, its precision is almost 100% with a sensitivity of 66%.

### ClusterCentroids (Undersampling) Model
![image](https://user-images.githubusercontent.com/96644316/178440854-9f5a8636-2ddb-476d-b7b7-a9ca00c7c9f5.png)  
![image](https://user-images.githubusercontent.com/96644316/178440892-3b6eb218-885a-4a37-ab41-fc3ab4758965.png)  
![image](https://user-images.githubusercontent.com/96644316/178440932-ccafe5a5-dc00-44a9-ab1f-a71e73dfeb91.png)  
* The balanced accuracy score is 52%.
* The high_risk precision is still 1% only with 63% sensitivity which makes a F1 of 1%.
* Due to the high number of false positives, the low risk sensitivity is only 40%.

### Smoteenn (Combination Over and Under) Sampling Model
![image](https://user-images.githubusercontent.com/96644316/178441106-1a4f8fd2-e8dc-48fb-a8b5-f91e40143266.png)  
![image](https://user-images.githubusercontent.com/96644316/178441131-48a832d8-9332-40bb-a93d-a7d4b764cda5.png)  
![image](https://user-images.githubusercontent.com/96644316/178441161-84be2561-5dc3-43b5-ac69-190e426237f4.png)  
* The balanced accuracy score is 62%.
* The high_risk precision is still 1% only with 68% sensitivity which makes a F1 of only 2%.
* Due to the high number of false positives, the low risk sensitivity is 57%.

### Balanced Random Forest Classifier Model
![image](https://user-images.githubusercontent.com/96644316/178441961-dc188988-295b-49aa-be26-358b5dd2e31f.png)  
![image](https://user-images.githubusercontent.com/96644316/178442023-c531faee-19fc-42b0-bf11-219d0f3106dc.png)  
![image](https://user-images.githubusercontent.com/96644316/178442072-cebccefb-436a-478b-b2e2-bd38ea9c2542.png)  
* The balanced accuracy score is 79%.
* The high_risk precision is still low at 4% only with 67% sensitivity which makes a F1 of only 7%.
* Due to a lower number of false positives, the low risk sensitivity is now 91% with 100% presicion.

### Easy Ensemble AdaBoost Classifier Model
![image](https://user-images.githubusercontent.com/96644316/178442319-52c0dcd5-75f8-4500-bfa1-0f7a1cef9676.png)  
![image](https://user-images.githubusercontent.com/96644316/178442358-f2509af0-463f-4e3a-b534-2a54c5842cb2.png)  
![image](https://user-images.githubusercontent.com/96644316/178442408-e0270572-3004-4305-b1b9-ec9ab6faf55d.png)  
* The balanced accuracy score is 93%.
* The high_risk precision is still low at 7% only with 91% sensitivity which makes a F1 of only 14%.
* Due to a lower number of false positives, the low risk sensitivity is now 94% with 100% presicion.

## Summary
Overall, the Easy Ensemble AdaBoost Classifier model was the most accurate and precise. This model would be best for determining credit risk due to it's accuracy score of 93%, low risk sensitivity of 94% and 100% precision.
