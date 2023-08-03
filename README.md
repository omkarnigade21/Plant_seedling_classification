# Plant_seedling_classification


Problem statement:
                To classify images of plant seedling. Dataset contains images of 12 types of plant seedlings. 
                

Approach:
1)	Build CNN based networks with conv(3X3) and maxpool(2X2) layers and experimented with changing parameters learning rate, number of layers, batch normalization, dropout ratio, etc.
2)	Used augmenter to increase number of images in each class. It is found that, overfitting is reduced with great extent using augmentation.
3)	Trained different image classification models with transfer learning.
4)	Compared results based on validation accuracy, validation loss and size of model(MB).

Results:
             Results of different models are tabulated below.       
             
Model              	Accuracy(%)	             Val_loss	                 Size(MB)	                Specifications	          
Model 3	                92	                    0.213	                  133	                  i/p shape=(120,120,3)                                                   	
Model 4	                92	                    0.28	                   69	                  i/p shape=(120,120,3)	                                                       
ResNet50	              96	                    0.0948	                 91	                  i/p shape=(224,224,3)                                                       	
DenseNet121	            86	                    0.38	                   28	                  i/p shape=(224,224,3)                                         	
InceptionV3	            38	                    1.765	                   98	                  i/p shape=(224,224,3)                                                                                  	
					
            Validation loss (categorical cross entropy) of ResNet50 model is much lesser than other models also it is giving highest accuracy of 96% on validation dataset and 99% accuracy on train dataset. Model is less overfit due to use augmentation.
            

