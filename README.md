# Sentiment-Analysis-and-Topic-Modeliing


## Descriptive Analysis of Datasets
The two cities we decided to analyze were Chicago and Nashville. To this we used the listings and reviews data from each city along with Covid-19 data for each state in which the cities are located. To summarize the datasets, we conducted exploratory data analysis to recognize trends and relationships within the datasets. First, we looked at a breakdown by room type for Airbnb’s in each city (Appendix 1). In both cities, entire homes/apartments made up most of the available accommodations. Next, we looked at the top hosts by property count (Appendix 2). In Chicago, one host owned over 500 properties, while no other owned over 100. In Nashville, 5 hosts owned over 100 properties. We then looked at average price by neighborhood (Appendix 3). 
We then turned our analysis to focus on the prices charged for each property. We found that Chicago has four neighborhoods with an average price over $300 while Nashville had six neighborhoods with an average price over $300 and two neighborhoods with an average price over $750. We also analyzed average price by room type (Appendix 4) and found that in Chicago entire homes had the highest average price, $245. In Nashville, hotel rooms had the highest average price, $998. Of 1,993 hosts in Chicago, 16 average a price over $1000. Similarly, in Nashville, 15 of 1,762 hosets had an average price over $1000 (Appendix 5). 6,334 of 7,414 Chicago properties had a price under $333, while 5,957 of 7,733 Nashville properties had a price under $330 (Appendix 6). To analyze the relationship between reviews and price, we plotted them on a scatterplot (Appendix 7). We found that as prices decreased, reviews increased. This makes sense because the lower price makes the properties more accessible allowing for more people to leave reviews. 
To visualize the relationship between Covid-19 and Airbnb we used the number of reviews as a proxy for stays and compared those to new Covid-19 cases in the states in which the cities we analyzed are located (Appendix 8). We found there to be a clear inverse relationship between the number of reviews and number of Covid-19 cases. We saw fewer reviews, and by our proxy stays, when there were spikes in Covid-19 cases.
Finally, we wanted to use the available latitude and longitude data to construct maps of each city and analyze the Airbnb properties based on location. The first map we constructed was a map with each circle denoting each Airbnb, the color of the circle denoted room type, and the size of the Airbnb denoted price (Appendix 9). This allowed us to visualize where the Airbnb properties were located and see where the more expensive ones were located. We then constructed a similar map but changed the size to reflect the number of reviews (Appendix 10). We observed less disparity in the number of reviews across the cities than there was in price. 
## Data Analysis
With sufficient data at our disposal through the form of customer reviews across cities like Nashville and Chicago, we decided to go ahead and check the major topics that would emerge out of a Topic Modelling exercise on the reviews. 
### Topic Modelling:

#### In Nashville we found out that the reviews were majorly based on the following topics:

<img width="250" alt="Picture 1" src="https://user-images.githubusercontent.com/28756098/212502409-9a478422-39a0-4fb9-8b64-1911c4b14a79.png">

Topic1= ['house','perfect','nashville','place','stay','home','space','beautiful','amazing’,’absolutely']

Meaning: Good and comfortable stay

<img width="250" alt="Picture 2" src="https://user-images.githubusercontent.com/28756098/212502411-93f0fa43-6050-4f9f-8b12-46a5c06a7383.png">

Topic2= ['stay','nashville','home','place','comfortable','clean','host','cozy','super','recommend']

Meaning: Perfect, amazing, and beautiful stay

<img width="250" alt="Picture 3" src="https://user-images.githubusercontent.com/28756098/212502412-2ede2344-fde9-457d-ad3a-252109b2e84f.png">

Topic3= ['great','place','stay','location','host','clean','recommend','great location','definitely','great place']

Meaning: Clean, comfortable, and home like stay

<img width="250" alt="Picture 4" src="https://user-images.githubusercontent.com/28756098/212502413-20780ce6-976b-43d3-9abf-b70d2a649915.png">

Topic4= ['great','location','easy','downtown','nashville','walk','clean','check','good','nice']

Meaning: Great stay, great location and place

<img width="250" alt="Picture 5" src="https://user-images.githubusercontent.com/28756098/212502414-78e90145-3a52-456e-972b-a3dc19ee1528.png">

Topic5= ['great','place','downtown','uber','close','stay','ride','distance','walking','quick']

Meaning: Downtown, great location, easy access

#### Similarly in Chicago we found out that the reviews were majorly based on the following topics:

<img width="250" alt="Picture 6" src="https://user-images.githubusercontent.com/28756098/212502416-5e0469b1-d931-4c2e-beb9-dc2bb697cc03.png">

Topic1= ['host', 'stay', 'place', 'chicago', 'room', 'good', 'time', 'house', 'home', 'airbnb']

Meaning: Good and comfortable stay

<img width="250" alt="Picture 7" src="https://user-images.githubusercontent.com/28756098/212502417-8bc4569a-cf50-411e-9511-3ded565dcde8.png">

Topic2= ['great', 'place', 'stay', 'location', 'clean', 'host', 'great location', 'nice', 'definitely', 'space']

Meaning: Great stay, great location and place

<img width="250" alt="Picture 8" src="https://user-images.githubusercontent.com/28756098/212502418-51e8039d-f2a8-45df-8b35-1ac3ef965bec.png">

Topic3= ['place', 'room', 'apartment', 'bed', 'nice', 'stay', 'great', 'kitchen']

Meaning: Nice apartment and home like stay

<img width="250" alt="Picture 9" src="https://user-images.githubusercontent.com/28756098/212502419-b74ed0ab-477c-4273-aa30-325eb6452b15.png">

Topic4= ['place', 'stay', 'neighborhood', 'comfortable', 'home', 'chicago', 'clean', 'apartment', 'great', 'quiet'] 

Meaning: Comfortable and clean stay, great location and place

<img width="250" alt="Picture 10" src="https://user-images.githubusercontent.com/28756098/212502420-bab34cf0-e402-4e60-afd5-e1c4a51cbcff.png">

Topic5= ['great', 'location', 'easy', 'place', 'highly', 'recommend', 'close', 'perfect', 'chicago', 'highly recommend']

Meaning: Great location, easy access, highly recommended

### Sentiment Analysis:

The next major exercise was to run a sentiment analysis across the various reviews. We generated Positive, Neutral and Negative scores for each reviews using the Sentiment Intensity Analyzer package in python and found out the share of reviews with positive sentiment and share of reviews with negative sentiment in both Nashville and Chicago.

#### The sentiment analysis exercise in Nashville generated the following insights:

![Picture 11](https://user-images.githubusercontent.com/28756098/212502421-4fe501a6-f2ab-4ba2-86c3-316b90c6c4e5.png) •	53% of customers gave high positive remarks about their stay

![Picture 12](https://user-images.githubusercontent.com/28756098/212502422-df3a87b1-4361-405c-b6e7-6da16c1773b1.png) •	43.1% of customers gave high neutral remarks about their stay

![Picture 13](https://user-images.githubusercontent.com/28756098/212502424-bdfc61f4-11cf-40db-b853-38aedcb5b855.png) •	0.05% of customers gave high negative remarks about their stay

#### In Chicago we came across the following insights following the sentiment analysis:

![Picture 11](https://user-images.githubusercontent.com/28756098/212502421-4fe501a6-f2ab-4ba2-86c3-316b90c6c4e5.png) •	49.7% of customers gave high positive remarks about their stay

![Picture 12](https://user-images.githubusercontent.com/28756098/212502422-df3a87b1-4361-405c-b6e7-6da16c1773b1.png) •	45.7% of customers gave high neutral remarks about their stay

![Picture 13](https://user-images.githubusercontent.com/28756098/212502424-bdfc61f4-11cf-40db-b853-38aedcb5b855.png) •	0.08% of customers gave high negative remarks about their stay

In general, we can see that Airbnb customers in Chicago are less satisfied on average when compared to their counterparts in Nashville. This is evident through the decrease in share of high positive remarks and increase in share of negative remarks in Chicago

<img width="391" alt="Picture 14" src="https://user-images.githubusercontent.com/28756098/212502425-9cd4506b-5c03-46e4-ba1e-f3d7fd13c331.png">

#### Covid Data Analysis with Customer Reviews:
From our analysis we have found out that Covid has peaked 3 times in the data we have considered, Dec 2020, Jan 2022, and Jun 2022. And we have also seen that during this time Covid had an inverse correlation with customer Airbnb bookings i.e., bookings jump when covid declines and go down when Covid peaks.

#### But we wanted to understand if Airbnb managed to do better from a company standpoint during this uncertain time period. For this we cross referenced the reviews before and after Covide started and came across the following findings:

<img width="275" alt="Picture 15" src="https://user-images.githubusercontent.com/28756098/212502426-b32a6022-de52-4c18-ad09-8d563e4e3182.png">

<img width="280" alt="Picture 16" src="https://user-images.githubusercontent.com/28756098/212502428-5051139e-0647-4f88-b6f0-3af451953d9c.png">

•	There has been a spike in positive scores during the Covid period in both Nashville and Chicago

•	There has been a slight reduction in negative scores during this time period 

•	There has been a significant reduction in the neutral scores during Covid period as opposed to earlier.

•	These factors indicate a shift in customer sentiment towards Airbnb during the covid period. The high standards of safety, cleanliness and precaution maintained by the Airbnb staff could be the reason for the positive outcome and the reason why the company was not severely impacted during the pandemic
