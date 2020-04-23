# Classification-of-the-102-Category-Flowers-Dataset
This was a group project that we did as part of completing a course
### Dataset
This dataset contains 102 classes. Each class has 40 to 258 images. Images are in different variations. Dataset can be downloaded [here](http://www.robots.ox.ac.uk/~vgg/data/flowers/102/index.html).

###Result
We have tried different approaches with this dataset. A comparison of all the approaches is shown below:<br>
![Comparison table](https://imgur.com/MSWT7qG.png)<br>
Based on the comparisons from table 1 we decided to take the small as out final model and ran it for
longer time. We ran our model for 50 epochs with early stopping condition. The condition was that if the
validation accuracy does not improve by 0.0001 in 5 epochs. Our training stopped after 23 epochs with
train accuracy of 100% and train loss of 9.8343e-04 and validation accuracy and loss being 53% and 3.54
respectively.<br>
![Loss](https://imgur.com/b3LwKXF.png)<br>
![Accuracy](https://imgur.com/5Ps6aof.png)<br>
The average test accuracy was 47% and the average over all class specific accuracies was 44%.The
average precision was 0.49.<br>
The confusion matrix and the number of classes per precision number is shown below:<br>
![Confusion Matrix](https://imgur.com/off9szK.png)<br>
![ Number of classes per precision value](https://imgur.com/SN3jons.png)<br>
Class specific accuracy and precision is shown below in respective graphs.<br>
![Accuracy of each class](https://imgur.com/cO2npvZ.png)<br>
![Precision of each class](https://imgur.com/1n0H8cK.png)<br>

###Cross Validation Results
We have tried cross validation with 10 folds. We used Scikit-learn’s StratifiedKFold() function to make
sure every class is equally proportionally present in both training and validation datasets. The maximum
and minimum test accuracy was 50% and 31% respectively. Among the 10 test results, the standard
variation was 0.0548 and the average was 47%.<br>
Accuracy from 1st to the 10th fold is visualized below:<br>
![cross-val](https://imgur.com/rnEiJPd.png)<br>

