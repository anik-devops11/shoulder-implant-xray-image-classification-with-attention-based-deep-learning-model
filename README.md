

# Shoulder implant X-ray image classification using Deep Learning

<p style="text-align: justify;">
This research addresses the critical task of classifying X-ray images depicting implanted shoulder prostheses for precise equipment selection and surgical planning. Utilizing the recently introduced SIXIC dataset our DenseNet-121 model integrating InceptionV3,EfficientNetB0, MobileNeV2,NasNetMobile and also a custom model enhances shoulder implant classification accuracy. The model employs a comprehensive feature extraction approach, leveraging the strengths of each architecture. We employ deep learning models and compare their performance to alternative classifiers such as CNN model. We find that deep convolutional neural networks outperform other classifiers significantly if and only if out-of-domain data such as ImageNet is used to pre-train the models. Experimental evaluations demonstrate its superior performance across key metrics and setting new benchmarks for shoulder implant classification. The proposed model’s high predictive performance positions it as a valuable tool for assisting in the treatment of injured shoulder joints. This research contributes significantly to medical image analysis specifically in the domain of shoulder implant recognition with promising implications for refined surgical planning and elevated patient care standards. The findings merit consideration for publication to disseminate insights and advance medical imaging research.</p> <br>

### Workflow for our Work

<p style="text-align: justify;"> This is the overall working process of our work.Firstly,we collect our dataset from online.Then, we split the dataset into training,testing and validation.The splitting ratio is 80-10-10.Next,we applied data preprocessing techniques such as image resizing,image normalization and label encoding. In image resizing we resizing our image into 180×180. In image normalization we scaled our pixel value.In label encoding  we use onehot encoding to convert into binary value.After preprocessing we applied data augmentation techniques to enhanced the dataset. After that we use deep learning model for feature extraction. Then, we compile our model to prepare it for training.After that,we train the model with using training and validation data and also evaluate the model based on the test data.And finally we classified our output.</p> <br>

![Logo](https://github.com/anik-devops11/shoulder-implant-xray-image-classification-with-attention-based-deep-learning-model/blob/main/Diagram/work%20flow.png)

<h3  align="center"> Workflow </h3> <br>

### Model Architecture

<p style="text-align: justify;"> This is our proposed model architecture select input image, at first we put Convolution layer for Extracting Features then  there are Max Pooling Layer which will extract Most Important feature from the input image. Then there comes multiple block of Dense Block and transition layer. In Dense Layer there are batch normalization to reduce sensitivity of the model and Convolution 3x3 layer. In the Transition layer there are 3x3 Max Pooling Layer ,Convolution layer and Batch Normalization. Then we comes to important portion of the architecture which Squeeze and Excitation Module. This module is introduced before the Dropout layer to improve feature learning capabilities which increase the model accuracy mainly. then after dropout layer there are Average pooling layer and a Fully Connected layer after all of these we got our desire output.</p> <br>


![Logo](https://github.com/anik-devops11/shoulder-implant-xray-image-classification-with-attention-based-deep-learning-model/blob/main/Diagram/DenseNet%20Model%20Architecture%20with%20SE%20Module%20Final.png)

<h3  align="center">Model Architecture </h3> <br>

## Feedback

If you have any feedback or queries, please reach me out at anikdasprivate@gmail.com