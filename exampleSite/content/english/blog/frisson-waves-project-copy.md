+++
date = 2021-08-31T15:00:00Z
description = "This project is a collaboration with yin. "
draft = true
image = "/images/frisson.jpg"
image_webp = "/images/frisson.webp"
title = "Emolleia Flowers"

+++
Emolleia Flowers project is to explore and design novel non-verbal interaction tools. We explore how to create expressive clothes and accessories that are able to instantaneously reflect our feelings.  We design a wearable kinetic display in form of three 3D printed flowers that can dynamically open and close at different speeds. Users can define their own animated motions. The kinetic display is the result of several design iterations trying to capture the movements of flower ensembles. We want to explore whether this type of wearable accessory could be a novel form of non-verbal communication.

The system we used in the frisson sharing concert is consisted of :

1. A physiological sensing wristband that records and extracts EDA and HRV that can be used to detect when someone has frisson.
2. A machine learning model that processes the wirelessly streamed physiological data for real time classification of the data as frisson or non-frisson.
3. A neckband with Peltier thermoelectric cooler modules (TEC) and vibro-tactile actuators which can trigger frisson.
4. A sharing server that controls the operation of all the devices and manages data processing and recording.
5. 

![](/images/frisson_concert2.jpg)

#### **Model Performance**

In order to train the model, we processed the recorded EDA and blood volume pulse (BVP) data as well as when the participants pressed the frisson-report button for data labeling. Our model was trained using the features extracted from a sliding window of one minute with one second overlap. The window was labeled as a frisson event if the button was pressed within the window.  We extracted four EDA features and three HRV features for training the model and applied leave one participant out cross validation (LOPO-CV) to divide data into training and testing sets. The classifier with the best performance presented an average accuracy score of 85.78% (sd = 11.23%).

![](/images/frisson_cm.jpg)

#### **Exploratory Analysis of the Physiological Dataset**

During the concert, half of the audience were wearing the devices for sharing frisson (neckband) while the other half were not. Besides comparing subjective feedback from the two groups, we also explored the physiological data collected and calculated the physiological synchrony (PS) of each group. PS occurs when the “physiological activity between two or more people” becomes associated or interdependent” and could be used as a feasible metric to quantify the experience of physiological connectedness. We conducted the decomposition into EDA tonic and EDA phasic, normalized the two components to remove individual differences, and processed dynamic time warping (DTW) to calculate the accumulated distance between every two persons in each group. Our findings may suggest wearing the neckband and sharing frisson could provide audience members more physiologically similar experiences in terms of short-term and sudden feelings of arousal compared with the long-term trend in certain concert sessions. _(submission under review)_

#### **See More Details in Related Publications**

_\[1\]_ He, Y., D. Zheng, G. Chernyshov, R. Thomsen, J. Han, D. Hynds, Y. S. Pai, K. Kunze, and K. Minamizawa. "Frisson Waves: Sharing Frisson to Create Collective Empathetic Experiences for Music Performances." In 2021 IEEE World Haptics Conference (WHC), pp. 591-591. IEEE, 2021.

_\[2\] Talks by Professor Kai Kunze: Frisson Waves - Augmenting Aesthetic Chills in Music Performances (_ [https://media.ccc.de/v/rc3-2021-fem-294-frisson-waves-augmentin](https://media.ccc.de/v/rc3-2021-fem-294-frisson-waves-augmentin "Frisson Waves - Augmenting Aesthetic Chills in Music Perfromances") ).

_\[3\] Article by Moonshot project_ ([https://cybernetic-being.org/works/frisson-waves/](https://cybernetic-being.org/works/frisson-waves/ "https://cybernetic-being.org/works/frisson-waves/")).

#### **Contributors**

Direction / Project Lead: Yan He  
Technical Direction / Engineering: George Chernyshov  
Data Engineering: Jiawen Han  
Performing: Muyu Liu / Danny Hynds / Yuehui Yang / Ragnar Thomsen / Yan He  
Technical Support: Dingding Zheng  
Research Supervisor: Kouta Minamizawa / Kai Kunze / Yun Suen Pai

#### **Special thanks**

J.Y.PLANNING / Studio Apollon / Jamie Ward / Kinga Skierś / Ziyue Wang / Qianqian Mu / Kanyu Chen / Matsuda Kento / Qing Zhang / Christopher Kim / Yulan Ju

#### **Funding**

###### Frisson Waves project is under the Cybernetic Being project supported by JST Moonshot.