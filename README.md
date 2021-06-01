<img src="img/Address Recommendation.png" />




# A description of the problem and a discussion of the background. 


## 1  _Business Understanding_

## 1.1 _Problem_

_Currently applications that are created to improve or facilitate people's lives are launched at all times. A possible idea to add to this group of applications would be the development of an ML model that provides a certain person the best place for them to move in a certain neighborhood. Suppose that a person wants to live in Ipanema in Rio de Janeiro, Brazil, and considers essential that near the new home should have restaurants, cafeterias and markets. Based on these preferences, the system would inform them what part of the neighborhood would be more compatible with the preferences. This project aims to divide certain neighborhoods into 5 areas and then analyze what is most common in the locations in each area, followed by a recommendation of the most compatible location based on the person's preferences._

## 1.2 _Interest_

_This application may be of interest to different market segments. Here I will mention two of them: the first is a real estate company trying to indicate to a person the most compatible location for them; the second is, for example, Google, where some people could provide their preferences and the Google maps could provide the best place for them to go after a hotel._

## 2  _Analytic Approach_

_The main problem is finding the best location that is most compatible with the person's preferences. In this case, I will use a composite model, where I will first try to apply a K-MEAN model to group the locations that are similar and then create a recommendation system based on the greater compatibility of the clusters with the person preferences. After I will provide the 5 most compatible locations for the person._

# A description of the data and how it will be used to solve the problem. 

_My data will be compound of two parts. The first is geographical coordinates, where i will use geopy or geocoder from google API to find the corresponding latitude and longitude of the neighborhood the person is looking to move in. After getting the main center of this neighborhood, i will create a circular area around this neighborhood, divide this area into many small pieces and get the respective latitude and longitude for each piece. The second part of the data will come from the application of the latitude and longitude data in the Foursquare API to get the venues inside each piece of my segmented area. With this data i will try to use a K-MEAN model so i can combine the regions that are similar. After the clustering of the regions, a recommendation system will be created based on information the person will give, like what are their preferences of things they judge to be important to have close to their new home._
