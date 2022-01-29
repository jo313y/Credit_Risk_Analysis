# Credit_Risk_Analysis

## Overview
Using data from LendingClub, a peer-to-peer lending services company, the target was to compare oversampling methods, undersampling methods, and combination sampling methods to determine which method works best for predicting credit risk. Next, two other methods that are built to reduce bias will be examined to determine which is better for predicting credit risk. The summary will provide overall what the best method to use for this task.

## Results
All of these results were taken looking at the prediction of the high credit risk. All of the methods predicted low credit risk almost perfectly. 

- Random Oversampling

![randomoversampling](https://user-images.githubusercontent.com/86981530/151679136-6e4c95db-d8e8-4e99-b471-d9de13c73372.PNG)

- SMOTE Oversampling

![smoteoversamplling](https://user-images.githubusercontent.com/86981530/151679147-6b7ed16d-9830-4552-baa9-af9d2d7cdca6.PNG)

- Cluster Centroid Undersampling

![clustercentroidunder](https://user-images.githubusercontent.com/86981530/151679162-784c135b-67d1-4f05-9d88-51fb025ce5fa.PNG)

- SMOTEENN Combination Sampling

![smotteencombination](https://user-images.githubusercontent.com/86981530/151679174-2c5f06ae-0ab4-4b95-a4b9-87864a0868a9.PNG)

- Balanced Random Forest Classifier

![balancedrandomforest](https://user-images.githubusercontent.com/86981530/151679182-3d6e7974-73f6-47c7-9965-5dd97f0e5af1.PNG)

- Easy Ensemble Classifier

![easyensembleclassifier](https://user-images.githubusercontent.com/86981530/151679186-4a2126a3-7736-4745-a4ac-db7623c210eb.PNG)

## Summary
There are a lot of ways to sample, test and use data to predict outcomes. This analysis was used to compare Random Oversampling, SMOTE Oversampling, Cluster Centroid Undersampling, and SMOTTEENN Combination Sampling. These were then compared to the Balanced Random Forest Classifier and the Easy Ensemble Classifier.

An ideal method will have the following: High Accuracy, High Precision, High Recall

Random Sampling, SMOTE Oversampling, CLuster Centroid Underampling had comparable accuracies overall at 0.66. The recall on the Random Oversampling, however, was slightly higher, which means there is less likely a chance for a false "high credit risk" predictions, which are actual "low credit risk". The SMOTTEENN Combination Sampling only had a 0.54 accuracy, but a 0.72 recall, which was the highest. Out of these four techniques, which are very comparable, the recommendation would be to not use SMOTTEENN Combination Sampling. 

The Balanced Random Forest Classifier and the Easy Ensemble Classifier are both better techniques than the previous four. They both have a lot higher accuracies. The Balanced Random Forest Classifier has a relative recall to the prevous four methods, but the Easy Ensemble Classifier has a higher accuracy, precisio, and recall. 


Easy Ensemble Classifier is easily the superiour technique when comparing credit risk. It has the highest accuracy, highest precision, and highest recall.
