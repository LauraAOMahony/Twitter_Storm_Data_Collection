# Twitter_Storm_Data_Collection
This project "Social Media and Named Storms", gathers relevant user posts on Twitter in order to demonstrate that social sensing can be used to detect and locate storm events. This repo describes the first part of the project, data collection. This involves navigating the Twitter Application Programming Interface (API) to collect raw data in the form of tweets containing keywords relating to named storms using the API. 

The Twitter API endpoint used allows to collect by keyword for a specified time period. Identifying relevant keywords allowed to identify relevant tweets. Twitter data for ex-hurricane Ophelia and storm Emma were collected using the Twitter API. Only original tweets in the English language containing at least on of these keywords were collected. The output of this collection process was over 4 million tweets pulled using the API saved in JSON format along with some metadata about the tweet such as username, timestamp, user location and geotag. 

Note: First need to apply for a Twitter developer account. A detailed application was required to show this project fell under the criteria required to get access to the academic product track licence needed to pull the necessary data from Twitter. This application can take up to several weeks to be approved. Medium post I wrote for people starting out Twitter API: [Getting Started with Data Collection Using Twitter API v2 in Less than an Hour](https://medium.com/p/600fbd5b5558)
 
Note 2: Output of this data collection is data that needs to be filtered and processed in the data processing stage of the project. This processing step is very important since the raw data collected is useless. This is because it is very poorly structured, and consists mainly of irrelevant content with no location attached. Data had to be geolocated also (vast majority of tweets contain no GPS coordinates). Filtering methods included a bot filter, basic relevance filter, machine learning filter (SVM), weather station filter, location filter. 

Command line snippets:
```
> cd YOUR_DIRECTORY_NAME

> set BEARER_TOKEN=YOUR_BEARER_TOKEN

> Jupyter Notebook
```
