+++
date = 2022-01-06T15:00:00Z
description = "online class streaming and hr sharing "
image = "/images/share_hr.jpg"
image_webp = ""
title = "HR Sharing as Connection"

+++
HR Sharing as Connection project explores the feasibility of sharing physiological data to enhance the connection between remote interactants. This project is under the Cybernetic Being project supported by JST Moonshot.

### Project Description

TInsufficient social cues between distributed learners in online learning could result in lack of engagement and social bonds. With the development of wearable sensing, sharing physiological data can be used to enhance mutual understanding and connectedness among sharers. Our work aims to explore the potential of sharing heart rate (HR) and heart rate variability (HRV) collected from distributed learners to enhance their online learning experiences. We implemented a physiological streaming system and conducted a field study with 11 learners in online classes.  Our exploratory results suggest streaming collective HR and HRV from multiple distributed learners could be used in online classes to improve engagement and sense of community.

### Field Study

We conducted a field study to investigate how distributed learners react to the streaming system that presents collective HR and HRV measurements in real time. Our system tracked Blood Volume Pulse (BVP) from self-built wrist-worn devices with an optical sensor placed on the fingertip referring to the set-up in previous work.

![](/images/device.jpg)

The device sampled the BVP at 50Hz and streamed to our system server via User Datagram Protocol (UDP), which supported distributed learners to stream their data without location restrictions.

We implemented glance-able line charts right below the presenter’s slide content  to avoid distracting learners from the class content. BPM was selected as an intuitive HR indicator of excitement and anxiety. While pNN50 was adopted as an established HRV feature to reflect relaxation and sustained attention.

![](/images/streaming_visual.jpg)

### Feedback

**_1. Motivation towards the Visual Streaming._**

All the participants reported they had the motivation to look at the streaming visual. Main reasons were the curiosity in others' reactions and the awareness of what’s going on in the class. Moreover, data contributors did not report privacy concerns with the sharing mostly because of the visual was shown in an aggregated manner and perceived anonymity.

**_2. Enhanced Engagement and Social Bond._**

Participants reported increasing engagement and sense of community with the streaming system.

a) Data contributors: Involved in the class more actively and felt more connected to ther distributed learners by seeing the data visualization.

b) Data viewers: a little hard to understand the system setup, such as how was the data recorded, integrated, and transformed. However, they were still interested in the trend and fluctuations of the streaming visualization

Survey results also showed perceived psychological engagement was slightly higher in the streaming session _(M = 3.99, SD = 0.38)_ than that without streaming _(M = 3.73, SD = 0.4)_, with a marginal significant difference _(t\[32\]= 1.95 , (.05 < p <.10))_.

### See More Details in the Related Publications

_\[1\]_ _Jiawen Han, Chi-lan Yang, George Chernyshov, Zhuoqi Fu, Reiya Horii, Takuji Narumi, and Kai Kunze. "Exploring Collective Physiology Sharing as Social Cues to Support Engagement in Online Learning." In 20th International Conference on Mobile and Ubiquitous Multimedia (MUM 2021), December 5–8, 2021_