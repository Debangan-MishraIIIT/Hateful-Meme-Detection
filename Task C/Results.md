### All Adam Optimisers (0.0005 lr for all)

1. Test Dataset<br>
accuracy: 0.678<br>
f1 score: 0.6581740976645435<br>
AUROC: 0.6786867773399652<br>
Recall: 0.6858407079646017<br>
Precision: 0.6326530612244898<br>

2. Dev Dataset<br>
accuracy: 0.65<br>
f1 score: 0.6170678336980306<br>
AUROC: 0.6529556650246304<br>
Recall: 0.6714285714285714<br>
Precision: 0.5708502024291497<br>

3. Test Unseen Dataset<br>
accuracy: 0.67<br>
f1 score: 0.5752895752895753<br>
AUROC: 0.65131283382419<br>
Recall: 0.5559701492537313<br>
Precision: 0.596<br>

4. Dev Unseen Dataset<br>
accuracy: 0.6425925925925926<br>
f1 score: 0.5234567901234568<br>
AUROC: 0.6182380779031671<br>
Recall: 0.5170731707317073<br>
Precision: 0.53<br>


### All Adam Optimisers (1e-4, 1e-4, 1e-5 for Text, Image, Total)

1. Test Dataset<br>
   accuracy: 0.653<br>
   f1 score: 0.6182618261826183<br>
   AUROC: 0.6554598893357269<br>
   Recall: 0.6706443914081146<br>
   Precision: 0.573469387755102<br>

2. Dev Dataset<br>
   accuracy: 0.634<br>
   f1 score: 0.6081370449678801<br>
   AUROC: 0.6352272727272728<br>
   Recall: 0.6454545454545455<br>
   Precision: 0.5748987854251012<br>

3. Test Unseen Dataset<br>
   accuracy: 0.65<br>
   f1 score: 0.5179063360881543<br>
   AUROC: 0.6237384711960983<br>
   Recall: 0.5356125356125356<br>
   Precision: 0.5013333333333333<br>

4. Dev Unseen Dataset<br>
   accuracy: 0.6481481481481481<br>
   f1 score: 0.5343137254901961<br>
   AUROC: 0.6249710379981465<br>
   Recall: 0.5240384615384616<br>
   Precision: 0.545<br>

### Changing the dropout values in final output model (0.2, 0.2, 0.3)
1. Test Dataset<br>
accuracy: 0.643<br>
f1 score: 0.6011173184357542<br>
AUROC: 0.6463844797178131<br>
Recall: 0.6641975308641975<br>
Precision: 0.5489795918367347<br>

2. Dev Dataset<br>
accuracy: 0.616<br>
f1 score: 0.5807860262008734<br>
AUROC: 0.6179340428672165<br>
Recall: 0.6303317535545023<br>
Precision: 0.5384615384615384<br>

3. Test Unseen Dataset<br>
accuracy: 0.644<br>
f1 score: 0.5014005602240896<br>
AUROC: 0.6157515876097269<br>
Recall: 0.528023598820059<br>
Precision: 0.47733333333333333<br>

4. Dev Unseen Dataset<br>
accuracy: 0.644<br>
f1 score: 0.5014005602240896<br>
AUROC: 0.6157515876097269<br>
Recall: 0.528023598820059<br>
Precision: 0.47733333333333333<br>


Model performs badly when SGD optimisation is used for the encoder models. With lower values of learning rates, the model does not converge quickly. Changing the structure of the model and increasing the depth too does not result in any improvements. When using dropout 0.5 for al the intermediate layers too fails. Various other hyperparameter changes may be done.