---
tags:
  - machine-learning
  - statistics
---
Accuracy is one metric for evaluating [[Classification]] models. Informally accuracy is the fraction of predictions our model got right. Formally, accuracy has the following defintions:

$$ Accuracy = \frac{Number\ of\ correct\ prediction}{Total\ number\ of\ prediction} $$

For binary classification, accuracy can also be calculated in terms of positives and negatives as follows:

$$ Accuracy = \frac{TP+TN}{TP+TN+FP+FN} $$

Where TP = True Positives, TN = True Negatives, FP = False Positives, and FN = False Negatives.

> [!example] Calculating accuracy for the model that classified 100 tumors as malignant (the positive class) or benigh (the negative class)
> 
></br><table><tr><td style = "background: green;"><p>True Positive (TP):</p><ul><li>Reality: Malignant</li><li>ML model predicted: Malignant</li><li><strong>Number of TP results: 1</strong></li></ul></td><td style = "background: red;"><p>False Positive (FP):</p><ul><li>Reality: Benign</li><li>ML model predicted: Malignant</li><li><strong>Number of FP results: 1</strong></li></ul></td></tr><tr><td style = "background: red;"><p>False Negative (FN):</p><ul><li>Reality: Malignant</li><li>ML model predicted: Benign</li><li><strong>Number of FN results: 8</strong></li></ul></td><td style = "background: green;"><p>True Negative (TN):</p><ul><li>Reality: Benign</li><li>ML model predicted: Benign</li><li><strong>Number of TN results: 90</strong></li></ul></td></tr></table>
$$Accuracy = \frac{TP+TN}{TP+TN+FP+FN} = \frac{1+90}{1+90+1+8} = 0.91$$
>The accuracy of this model is 91% but the model isn't doing a great job. If you look closely, out of 100 tumor example, 91 are benign and 9 are maligant. </br>
>Out of 91 benign tumors, the model accurately identify 90 as benign. That's good. However, of the 9 malignant tumors, the model only correctly identifies 1 as malignant. Which is terrible

Accuracy alone doesn't tell the full story when you're working with a [[class-imbalanced data set]]. 














