# RT-Q-CNN
# Vedat TUMEN
Road Type and Quality CNN Project

To develop effective advanced driving assistance systems, it is important to accurately recognize current driving environments and make critical decisions about driving processes. The prevention of accidents through the interaction of the driving assistance systems with the environment and ensuring optimum driving dynamics are the main topics in this field. Vehicles need to recognize the road type and quality at a high accuracy to ensure the most suitable driving for the road type. It is also important to use both uncomplicated and cost-effective systems when performing this detection. In this study, a deep learning-based approach that can be used in vehicle driver assistance systems is proposed for the automatic recognition of road type and quality. In this approach, it is possible to determine the road type and the quality of the road using only driving images as the input data. A new convolutional neural network model is designed for classification of the driving images. Driving images obtained from Google Street View are used to evaluate the recognition system for the actual driving environment. The proposed approach shows that the road types were determined with accuracy of 91.41%, and the pothole road–smooth road distinction was successful at 90.07%. It can be said that the proposed method is an effective structure that can be used for advanced driving support systems, V2I communications systems, and similar intelligent transportation systems.

In this Project two different experimental studies were performed. The first was an automatic classification of the road type. In this experimental study, image data of five classes (Class-A-B-C-D-E) were used. The second experimental study was to determine the road quality. In the second experimental study, a Class-F data set containing distorted road images and a mixture of Class-A-B-C-D-E non-distorted images was used. Furthermore, under each experimental study, two different datasets were used. The first of these includes images without any preprocessing, and the dimensions of the images in the dataset were resized as 128×128, passed through the model, and their performance was evaluated. In the second dataset, the images were passed through a designed filter using the VP method, and only the horizontal side of the vanishing point was cropped according to the optimum vanishing point. A single CNN model was used in all experimental studies. This CNN model is a new model designed for this work and is called RTQ-CNN, as mentioned previously. This model was applied to the dataset, and the classification performance was evaluated. 

 My dataset is https://drive.google.com/open?id=1cTRTblLZT-sUU7EtHVUv6ilBrQwGbfTk


# Results:
  Models	                  Road Type Classification Accuracy 	                          Road Quality Classification Accuracy
	                      Raw Images  	Pre-Processed Images with VP	                Raw Images        Pre-Processed Images with VP
  Vgg_8	                    71.88%	               88.28%	                              83.93%	                      82.14%
  Vgg_6	                    80.47%	               89.06%	                              85.71%	                      89.29%
  LeNet_5	                  80.47%	               89.06%	                              83.93%	                      87.50%
  Vgg_5	                    81.25%	               89.84%	                              83.93%	                      89.29%
 Proposed RTQ-CNN	        81.42%	               91.41%	                              87.50%	                      91.07%
