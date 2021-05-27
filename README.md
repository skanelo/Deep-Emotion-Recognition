# Deep-Emotion-Recognition
EfficientNet model is fine-tuned on facial expressions to detect 6 of the basic emotions <br>
(i.e. **anger, disgust, fear, happiness, sadness, surprise** according to [Ekman and Friesen](http://www.communicationcache.com/uploads/1/0/8/8/10887248/constants_across_cultures_in_the_face_and_emotion.pdf)).

The **CK+48** dataset has been used (for both training and testing), and the model achieved <br>
*97.84%* validation accuracy, and *96.43%* accuracy on a test set that it had not seen during the training phase again.

Below the predictions of the network on some randomly chosen images from the test set are presented. These images <br>
belong to the test set, and thus during the inference mode it was the first time the model encountered these samples.

<img src="https://github.com/skanelo/Deep-Emotion-Recognition/blob/main/results/pred_2.png" width="400"> |
<img src="https://github.com/skanelo/Deep-Emotion-Recognition/blob/main/results/pred_3.png" width="400"> 

The predictions of the model as well as a barplot of its confidence is presented on these images along with the actual label of each image.<br>


<br>The model achieved those results in almost no time (<3minutes), in less than 50 epochs (best val_accuracy was saved in the 46th epoch)
and with a few examples (927 samples in total for training, validation and testing). The learning curves are also presented below:

<img src="https://github.com/skanelo/Deep-Emotion-Recognition/blob/main/results/learning_curves.png" width="850" height="360"> 

A more comprehensive analysis of my approach as well as a step-by-step guide is presented at my **<pending_hyperlink_for_the_article>** on Towards Data Science.
