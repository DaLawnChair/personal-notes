### $Accuracy = \frac{\text{correct classifications}}{\text{all classifications}} =\frac{TP + TN}{TP + TN + FP + FN}$
* "how many of your guesses are correct"
* Not the best metric because many times, you can always guess 1 class and get most of it right if you guess the most common classes
* Bad for imbalanced datasets

### $Precision = \frac{\text{correctly classified actual positives}}{\text{everything classified as  positives}}=\frac{TP}{TP + FP}$
* aka positive predicted value (PPV)
* ratio of relevant retrieved instances over all retrived instances
* "how well you can find true positives(TP) out of all positive predictions"
* Use when it's very important for positive predictions to be accurate.

### $\text{False Positive Rate} = \frac{\text{incorrectly classified actual positives}}{\text{all actual negatives}}=\frac{FP}{FP + TN}$
* Aka FPR
* Use when false positives are more expensive than false negatives.

### $Recall = \frac{\text{correctly classified actual positives}}{\text{all classified positives}}=\frac{TP}{TP + FN}$
* aka sensitivity, true positive rate (TPR)
* "how well you can find true positives(TP) out of all correct predictions(TP+FN)"
* Use when false negatives are more expensive than false positives.
### $Specificity = \frac{\text{number of true negatives}}{\text{total number of negatives}}=\frac{TN}{TN + FP}$
* aka true negative rate (TNR)
* "how well you can find true negatives(TN) out of all negative predictions(TN+FP)"


Precision improves as false positives decrease, while recall improves when false negatives decrease.

#### $F1 = \frac{\text{2 x Precision x Recall}}{\text{Precision x Recall}}$
* balance between precision and recall
* most general metric for evaluating models
* F1 high implies both are high

##### $\text{Average Precision} = \int_{0}^{1}P(R)dR$
* Effectively AUC of the Precision-Recall Curve
* mAP is just the average precision for all IoU intervals for all classes

##### $mAP = \frac{1}{n} \sum_{k=1}^{k=n} AP_{k}$
* where Ap_k is the AP of the class k
* n is the number of classes

Confusion Matrix:
* representation of TP,TN,FP,FN 

Threshold: a numerical value deciding the minimum probability needed for a prediction to be counted as positive, otherwise it is negative
* In classification, this is used to segregate predictions
* In object detection, this is used to threshold the minimum IoU for the model to accept it as a detection
##### $IoU = J(A,B) = \frac{|A \cap B|}{|A \cup B|}$
* intersection over union
* IoU assesses the intersection of two bounding boxes (the predicted one and ground truth box)
* Derived from the Jaccard index. 
* Note that this and all the derivatives are NOT used during training, because the IoU will be terrible when a model doesn't output anything, so its will be 0, so no proper gradients for the network

**Precision-Recall curve** is obtained by plotting the model's precision and recall values as a function of the model's confidence score threshold.
* encapsulates the tradeoff of both metrics and maximizes the effect of both metrics
* downward sloping, since lowwer confidence implies more predictions (more recall), and fewer correct predictions made (lowers precision)
	* Upward sloping is ussually a bad sign
* “When a model has high recall but low precision, then the model classifies most of the positive samples correctly but it has many false positives(i.e. classifies many Negative samples as Positive).“
* “When a model has **high precision but low recall**, then the model is accurate when it classifies a sample as Positive but it may classify only some of the positive samples.”


ROC 
* reciever operator characteristic
* calculates TPR and FPR at thresholds
AUC-ROC:
* area under the ROC curve
* represents the probability that the model, if given a randomly chosen positive and negative example, will rank the positive higher than the negative
* In more concrete terms, a spam classifier with AUC of 1.0 always assigns a random spam email a higher probability of being spam than a random legitimate email. The actual classification of each email depends on the threshold that you choose.
* Can be used to compare models if the datasets are roughly balanced
* Higher the AUC the better
* Pick points that minimize your concern
	* Ie if you don't want false positives (ie cancer classification), pickpoints with a lower FPR. This might cause the model to do worse in TPR though
* AUC < 0.5 means its worse than chance


AUC-PRC:
* area under the Precision-Recall curve
* Can be used to compare models if the datasets are imbalanced
* Higher the AUC the better

Prediction Bias:
* the difference between the mean of a model's predictions and the mean of ground-truth labels in the data.
	* Zero prediction bias
		* 5% of emails are spam in dataset-> model should classify 5% of emails as spam
	* Having a prediciton bias that is off is bad
* Causes of bias
	* Biases or noise in the data, including biased sampling for the training set
	- Too-strong regularization, meaning that the model was oversimplified and lost some necessary complexity
	- Bugs in the model training pipeline
	- The set of features provided to the model being insufficient for the task

sources: 
https://www.v7labs.com/blog/mean-average-precision
https://developers.google.com/machine-learning/crash-course/classification/roc-and-auc#:~:text=The%20ROC%20curve%20is%20a,holdover%20from%20WWII%20radar%20detection. -> ROC and ROC-AUC