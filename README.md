# MLJHP
Repository for John Hopkins Practical Machine Learning Course
## Preparation  
Prepare two data frames one for each file(training and testing)

Background for the variable classe
It corresponds to Unilateral Dumbbell Biceps Curl in five different fashions: according to the specification (Class A), throwing the elbows to the front (Class B), lifting the dumbbell only halfway (Class C), lowering the dumbbell only halfway (Class D) and throwing the hips to the front (Class E). Class A corresponds to the specified execution of the exercise, while the other 4 classes correspond to common mistakes. 
Generate an Histogram to see the frequencies of the classe variable.

Eliminate the features with NA, from both sets(training and testing)
Eliminate some features that don't contribute to the model we are planning to create

## Summary
After reviewing the available information in the site for the "Human Activity Recognition", in particular the document available in
"http://groupware.les.inf.puc-rio.br/public/papers/2013.Velloso.QAR-WLE.pdf".
The strategy was based in generating 4 subsets one for each sensor;
ARM, BELT, DUMBBELLL and FOREARM.
The goal was to seek the features that were common among all sensors with a significant contribution to their corresponding model. With this set of features, a new model will be created for prediction. Our requirements were to have a much smaller set of features than the original 159 (without classe). We would like to have fewer than 16 (an empiric number to make the computational times acceptable) 

For each sensor a model was built the corresponding rfcv was used to assist in checking the model.
