# Neural Network for Binary Classification of flower Rose and Sunflower

The dataset contains 2400 images of flowers. The data collection is based on the data flickr, google images, yandex images. You can use this dataset to recognize flowers from the photo. The pictures are divided into two classes: rose and  sunflower. For each class there are about 1200 photos.
 
Total data: 2400 images <br/>
Train data: 50% of total data <br/>
Validation data: 25% of total data <br/>
Test data:  25% of total data <br/>

Model no. | Model Architecture | Epoch vs train & Val accuracy plot | Train accuracy | Validation accuracy | Test accuracy
--- | --- | --- | --- | --- | ---
1 | CNN2D | Figure 1.0 | 99.48% | 90.67% | 98.67%
2 | CNN2D with Drop out | Figure 2.0 | 99.70% | 88.67% | 98.67%
3 | CNN2D with BatchNormalization | Figure 3.0 | 99.78% | 89.56% | 97.83%
4 | VGG16 | Figure 4.0 | 100% | 94.89% | 99.00% 
 
 
## Figure 1.0
![alt text](https://github.com/krishnapal2545/NNFL_FlowerClassification/blob/master/Accuracy_vs_Epoch_Plot/FirstModel.png?raw=true)

## Figure 2.0
![alt text](https://github.com/krishnapal2545/NNFL_FlowerClassification/blob/master/Accuracy_vs_Epoch_Plot/SecondModel.png?raw=true)

## Figure 3.0
![alt text](https://github.com/krishnapal2545/NNFL_FlowerClassification/blob/master/Accuracy_vs_Epoch_Plot/ThirdModel.png?raw=true)

## Figure 4.0
![alt text](https://github.com/krishnapal2545/NNFL_FlowerClassification/blob/master/Accuracy_vs_Epoch_Plot/FourthModel.png?raw=true)

## Conclusion

Our custom CNN models can achieve 98.67% accuracy on test data. By adding batch normalization layer and dropout layer, we solved the problem of overfitting and found 97.83% and 98.67% test accuracy respectively. Also, we can get better results by making our initial network deeper which means depth of network matters a lot. VGG achieves high train and test accuracy with a batch size of 32. The changing of batch size influences the results a lot. With too small or too large batch size, training process stucks at a local min point and the accuracy is low. It also shows the result of overfitting as train accuracy is much higher than validation and test accuracy.
