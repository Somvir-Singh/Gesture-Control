Experiment Number	Model	Result 	Decision + Explanation
1	Conv3D	Training Accuracy =90.34%
Validation accuracy =75%	Increasing the no of frame and epoch
2	Conv3D	Training Accuracy =95.72%
Validation accuracy =100%	Model is overfitting –we reduce no of parametes – also a padding in conv3d and a filter of (3,3,3)
3	Conv3D	Training Accuracy =94.11%
Validation accuracy =37.5%	Adding one more convolution layer 
4	Conv3D	Training Accuracy =95.72%
Validation accuracy =75%	Rerducing kernel to (2,2,2) also doing batch normalization before Pooling
5	Conv3D	Training Accuracy =98.39
Validation accuracy =50%	Model is overfitting . switching architecture to Conv2D +LSTM
6	Conv2d+LSTM	Training Accuracy =98.87%
Validation accuracy =87.5%	Reduce Cropping


7	Transfer learning with LSTM	Training accuracy =100%
Validation accuracy =100%	Overfitting 
Final Model	Model 6		
After doing all the experiments, we finalized Model 8 – Conv2D+LSTM, which performed well.

Reason:

1.	Training Accuracy : 98%, Validation Accuracy : 87%
2.	Number of Parameters(3,084,133)less according to other models performance
3.	Learning rate gradually decreacing after  21 Epoch
