# Youtube-API-Analyzer
[Project code](youtube_videos_analyzer_EDA.ipynb) using the YouTube API to analyze information about channels
related to the world of information technology (IT) in order to obtain valuable information
needed by a future content creator who wants to start a new channel on the platform


## Introduction

Founded in 2005, Youtube has grown to become the second largest search engine in the world (behind Google) that processes more than 3 billion searches per month. [[1]](https://www.mushroomnetworks.com/infographics/youtube---the-2nd-largest-search-engine-infographic/). It is, however, generally a myth how the Youtube algorithm works, what makes a video get views and be recommended over another. In fact, YouTube has one of the largest scale and most sophisticated industrial recommendation systems in existence [[2]](https://dl.acm.org/doi/10.1145/2959100.2959190). For new content creators, it is a challenge to understand why a video gets video and others do not. There are many "myths" around the success of a Youtube video [[3]](https://vidiq.com/blog/post/5-youtube-algorithm-myths-youtubers-need-to-know-about/), for example if the video has more likes or comments, or if the video is of a certain duration. It is also worth experimenting and looking for "trends" in the topics that Youtube channels are covering in a certain niche.

As a System Information Engineering Student who right now is traning in Data Analysis and consuming Youtube Resources for learning, I decided to gain some insights on this topic which might be useful to put in practice the technical and theoretical knowledge seen during my career in college. The scope of this small project is limited to Programming and Software Engineering channels I follow and I will not consider other niches (that might have a different characteristics and audience base). Therefore, in this project I will explore the statistics of around 10 Youtube channels I'm subscribed to related to the world of IT

## Aims and Objectives

Within this project, I would like to explore the following:

- Getting to know Youtube API and how to obtain video data.
- Analyzing video data and verify different common "myths" about what makes a video do well on Youtube, for example:
    - Does the number of likes and comments matter for a video to get more views?
    - Does the video duration matter for views and interaction (likes/ comments)?
    - Does title length matter for views?
    - How many tags do good performing videos have? What are the common tags among these videos?
    - Across all the creators I take into consideration, how often do they upload new videos? On which days in the week?
- Explore the trending topics using NLP techniques
    - Which popular topics are being covered in the videos (e.g. using wordcloud for video titles)?
    - Which questions are being asked in the comment sections in the videos
 
## Steps of the Project
1. Obtain video meta data via Youtube API for 10 channels in the IT niche (this includes several small steps: create a developer key, request data and transform the responses into a usable data format)
2. Prepocess data and engineer additional features for analysis
3. Exploratory data analysis
4. Conclusions


## Data Selection

As this project is particularly focused on channels of my preferences, I found that not many readily available datasets online are suitable for this purpose. 

So, I created my own dataset using the [Google Youtube Data API version 3.0](https://developers.google.com/youtube/v3). The exact steps of data creation is presented in section *2. Data Creation* below.

## Data Limitations

The dataset is a real-world dataset and suitable for the research. However, the selection of the 10 Youtube channels to include in the research is purely based on my knowledge of the channels in IT field and might not be accurate. In addition, this is a personal analysis of channels that seems interested to me and I watch their content every day so there might be tons of other channels that might also very interesting to look into, which could be the next step of this project.

## Ethics of Data Source

According to [Youtube API's guide](https://developers.google.com/youtube/v3/getting-started), the usage of Youtube API is free of charge given that your application send requests within a quota limit. "The YouTube Data API uses a quota to ensure that developers use the service as intended and do not create applications that unfairly reduce service quality or limit access for others. " The default quota allocation for each application is 10,000 units per day, and you could request additional quota by completing a form to YouTube API Services if you reach the quota limit.

Since all data requested from Youtube API is public data (which everyone on the Internet can see on Youtube), there is no particular privacy issues as far as I am concerned. In addition, the data is obtained only for research purposes in this case and not for any commercial interests

## References/ Resources used:

[1] Youtube API. Avaliable at https://developers.google.com/youtube/v3

[2] Converting video durations to time function. https://stackoverflow.com/questions/15596753/how-do-i-get-video-durations-with-youtube-api-version-3

[3] P. Covington, J. Adams, E. Sargin. The youtube video recommendation system. In Proceedings of the Fourth ACM Conference on Recommender Systems, RecSys '16, pages 191-198, New York, NY, USA, 2016. ACM
