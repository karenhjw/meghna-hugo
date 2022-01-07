+++
date = 2019-03-31T15:00:00Z
description = "This project is about emotion recognition via digital pen and handwritings. "
image = "/images/pen.jpg"
image_webp = ""
title = "Sentiment Pen "

+++
Sentiment pen project is to investigate the possibilities of emotion recognition via daily life activities -- writing and drawing. The proposed concept exemplifies how a digital system could recognize the emotional context of the interaction. 

#### Project Description

Handwriting is a widespread example of such an activity. Handwriting is a tradi- tionally non-digital way of recording information and conveying it to others. With the advent of the digital era, digital pens or styli allow users to digitize their writings and drawings instantly and store them on their digital devices. Digitized handwriting gives us access to precise handwriting data without requiring computer vision. Every stroke’s data can be recorded and emotion-related features can be extracted as the user writes or draws. We discuss our approach to emotion recognition and the underlying neuro- physiological mechanisms of handwriting (e.g. autonomic nervous system, muscle memory ).  

We collected labelled data where participants were asked to perform simple writing tasks after being exposed to a series of emotionally-stimulating video clips from The Emotional Movie Database (EMDB) one set of four clips per each quadrant on the circumplex model of emotion. The user-independent Support Vector Classifier (SVC) built using the recorded data shows up to 66% accuracy for certain types of writing tasks for 1 in 4 classification (1. High Valence, High Arousal; 2. High Valence, Low Arousal; 3. Low Valence, High Arousal; 4. Low Valence, Low Arousal).

#### Model Performance

Excluding stroke start and end time we analyzed the remaining 40 features in order to test whether there is any relation between the handwriting features and the self-reported emotional state of the participant recorded using the SAM. In order to do this we used the C-Support Vector Classification (SVC) from scikit-learn library with valence, arousal and dominance ratings as labels. In order to select the most promising features we have calculated the Gini Importance for each feature for each of the three tasks separately. Then selected and combined top 10 features from each of the tasks.

The score results of this classification are presented on the figure below. We ran classification on the data sets from each task and on all three tasks combined. It was found that the classification precision changes greatly if we use only short or only long strokes. The stroke data was split into short and long strokes in relation to the median for each data set used. Short strokes gave particularly good results for task 3, as it required participants to draw mostly short lines. Accuracy for this test is reaching 66% for 1 in 4 groups classification. Using long strokes showed better results for tasks 1 and 2 with accuracy of 50 and 51% respectively. Surprisingly, the accuracy of classification of the short stroke data set for all 3 tasks was higher than for long stroke data set (47% for short and 35% for long).

![](/images/independent.jpg)

### Related Publications

_\[1\]_ Han, Jiawen, George Chernyshov, Dingding Zheng, Peizhong Gao, Takuji Narumi, Katrin Wolf, and Kai Kunze. "Sentiment pen: Recognizing emotional context based on handwriting features." In _Proceedings of the 10th Augmented Human International Conference 2019_, pp. 1-8. 2019.