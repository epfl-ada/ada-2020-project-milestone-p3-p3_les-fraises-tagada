#### Authors: Marion Chabrier, Clement Lion, Michael Spierer

# Milestone P3:

### 1. Title: Cultural differences in mobility

### 2. Abstract
Brightkite and Gowalla are mostly american social networks. Therefore, if the paper *“Friendship and mobility”* gave meaningful results, we don’t know if they translate well to other countries. Moreover, they are very theoretic. We want to find practical advices that we can give to a foreigner visiting a country. In our project, we will on comparing results across countries by using the dataset from the location-based social media Foursquare. The dataset contains the position of Checkins for each user and friendship relationships. We want not only to study friendship (distance between friends' houses, do friends travel to see each other) but also the most popular Points of Interest per country. This can be possible because our dataset of Checkins associates a point of interest to each location. Since working on our full dataset seems to be challenging due to its size, we propose to split our data by geographic location.

### 3. Research questions

* What are the differences in mobility patterns across countries ?
* What are the friendship behaviours of users depending on their countries ?
* Which Places Of Interest (POI) are we the most willing to move to ?
* Can we predict the next POI a user will move to, knowing which previous POIs he visited ?


### 4. Proposed datasets

“Global-scale Check-in Dataset with User Social Networks” from two research projects at this address (project 5 by Dingqi Yang): ( https://sites.google.com/site/yangdingqi/home/foursquare-dataset#h.p_7rmPjnwFGIx9). The dataset is coming from Foursquare and it contains the information of 22,809,624 checkins by 114,324 users, 607,333 friendship links and 3,820,891 POIs. It is approximately twice as big as the other dataset. It also contains a set of worldwide check-ins with country flags taken over about two years and two snapshots of the corresponding user social network before (in Mar. 2012) and after (in May 2014) the check-in data collection period. In order to use it, we will need to merge and compare these different databases to transform it to obtain a dataset that looks like the one of Gowalla and Brightkite.

### 5. Methods

**Data collection:**  We need to merge our new dataset of check-ins with our new dataset of POIs since it comes as two big files. One containing the check-ins of a user with a timestamp and a location key and the second table a location key and information about latitude and longitude of a location. Hence, we will need to merge those two sets. Since they are very large, we might want to separate them in smaller subsets according to geographical zones.

**Comparing mobility patterns:** We want to focus on differences between countries. Therefore, for each country, we will compute statistics on mobility (distance between friends homes and see for which country we have friends that live far away)...

**Identifying interest of users:** We want to see how many friends users of different countries have. Since we have the chance to match each cell to a POI, we want to identify what are the most popular points of interests by geographic zone. We also want to identify which combinations of POIs often visited (do users go to a coffee shop after going to the office ?). This is bound to reveal interesting cultural differences.


### 6. Proposed timeline


**Week 1:**  downloading of the foursquare datasets, and merging our dataset of check ins with our dataset of POIs. Since they are very large, we will need to separate them in smaller subsets according to geographical zones like the US, Western Europe...

**Week 2:** Comparing mobility patterns in small subsets. (distance between friends' homes by countries) and begin the implementation of interest of users.


**Week 3:** continuing with analysis, attempting at finding a mobility model, preparing the data story and short video.


### 7. Organization within the team

* Clement will focus on cleaning the data by splitting the data by countries, merging them and adding appropriate columns. The resulting datasets will then be shared before the end of week one. During the next two weeks, Clement will then work on the POIs to identify the most popular points of interest per country, which one users are the most probable to go to and from this, he will attempt to create a mobility model. Parallel to that, Clement will start working on the data story.

* Marion will, in the first week, begin by finding the positions of user's house by inspiring herself of what was done in milestone P2. In week two, she will integrate the algorithms with the countries subsets made by Michael and Clement. In week 3, she will focus on preparing all needed figures and examples for the part she prepared. At the same time Marion will also prepare the short video with the main ideas.

* During the first week, Michael will work on cleaning the data and merging the datasets and then splitting the data according to the geolocation. During the second week, Michael will work on creating the website that will host the data story. Finally last week, he’ll work on storytelling and on a good way to present the research.     


### 8. Notebooks

The Github repository contains one notebook. Run all cells one after the other to make it work.



