# Credit Risk Analysis

## Overview  

The presenta analysis has as an objective to test the different methods available and detemrmine which of them is best suited to predict credit risk, based on the statistical results for each.

## Results

### Random Oversampling

![Random Oversampling](https://user-images.githubusercontent.com/89816213/151717189-4c0f31e1-9945-4346-ac92-d8e5eb157211.PNG)

Given that we are considerning a universe in which most accounts are not considered of High risk, we could get some omissions if we take samples randomly, so we make sure that there is an important representation of the lesser category by oversampling. This method has a precission of 1 but a precission oof onluy 0.01 for risky opperations, while having a sensitivity of 0.7 for riisky accounts.

### SMOTE Oversampling

![SMOTE Oversampling](https://user-images.githubusercontent.com/89816213/151721140-301ca535-d01b-46cb-be7b-d067982a4b29.PNG)

SMOTE oversampling involves increasing the number of appereances of the lesser category by adding "synthetic" members of this group. As we can see, it has an even lower sensitivity than the random oversampling method.

### Undersampling

![Undersampling](https://user-images.githubusercontent.com/89816213/151721165-8156bd31-faa0-40dd-a46a-e99e954969d7.PNG)

Undersampling involves the opposite process, in this scenario we diminish the number of the higher category in comparisson to the lesser category. This method has a precission of zero and a low sensitivity.

### SMOTEEN

![SMOTEEN](https://user-images.githubusercontent.com/89816213/151721180-aa579736-e76d-44d9-be59-400f542cefe2.PNG)

this method combines both over and undersampling, as we can see it has a relatively high sensitivity when compared with the other methods.

### Random Forest

![Random Forest](https://user-images.githubusercontent.com/89816213/151721188-6759d4fb-8fa8-47d0-a9f1-b976962a132f.PNG)

![Random Forest importance](https://user-images.githubusercontent.com/89816213/151721202-5b68e856-1984-4a9c-9d5e-8cf99faf30e8.PNG)

The random forest has a high precission, which can be attractive at first, but it's sensitivity is relatively low. 

### adaBoost

The adaBoost mehtod shos a sensitivity too low, and the precission for the hihg risk accounts is of 50% (basically a coin flip.

## Summary

The method with the best degreee of safety is SMOTEEN, since it has a higher sensitivity and therefore diminishes the risk of fraudulent operations being accepted.

