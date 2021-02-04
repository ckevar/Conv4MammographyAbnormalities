# Convolutional Neural Network for Medical Imaging Analysis - Abnormality

The project was developed as final project for the Computational Intelligence course. The classifiers are built from scratch or pretrained models such vgg16 and incepcionV3. and one awesome ensemble system. the CI_project holds the entire documentation and if you have problems accessing the files, let me know.
The Classifiers are as follows:


* **Scratch_CNN_2classes** design of a from-scratch classifier to discriminate among Masses and Calcifications.
* **Scratch_CNN_4classes** design of a from scratch classifier to discriminate among benign mass, malignant mass, benign calcification and malignant calcification.
* **Pre_Trained_2classes** design of a pre-trained models, a comparison between vgg16 and InceptionV3 as full-fine-tune and feature-extractor-only to discriminate among mass and calcification.
* **Pre_Trained_2classes** design of a pre-trained models, a comparison between vgg16 and InceptionV3 as full-fine-tune and feature-extractor-only to discriminate among benign mass, malignant mass, benign calcification and malignant calcification.
* **BaselineCNN** design of context-based classifier to discrimate masses and calcification. it compares InceptionV3 as siamesse and full-fine-tuned model.
* **Ensemble** Several mathematicals models are proposed  to merge the output of the following models _Scratch_CNN_2classes_, _Pre_Trained_2classes_ and, _BaselineCNN_. Such math models were: Average, Accuracy-based Weighted average, Logic Voting (inspited in Redundancy Engineering), Precision-based Weighted Average and, Opinion Rating.
## Opinion Rating Approach as Ensemble system
the idea behind this approach is to ignore as much as possible the net's output around 0.5, and emphasize or keep the values close to 1 and 0, because the last values define the classification. For such purpose, three equations were analysed. _tan_, _sinh_, _3-degree polynomial_, _5-degree polynomial_, _29-degree polynomial_ and, _63-degree polynomial_. The large polynomial values were used to understand how much outputs around 0.5 can be considered meaningless before compromise the good performance. 
