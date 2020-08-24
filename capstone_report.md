# 1 Introduction

## 1.1 Background

This project will make use data science analytics to guide a new business project.

## 1.2 Business Problem

A client would like open an Italian restaurant in the downtown area of Toronto. They would like to know which neightbourhood would be best to open a new restaurant. The client is opening a more upscale restaurant so would not like to compete with other Italian restaurants in the area.  They would also like to be in an area where there is a good choice of nightlife attractions in the hope customers would most likely look for some place to eat first and then go out afterwords while in the area.

In summary the customer is looking for:

- Downtown Toronto location.
- Area with other types of restaurants.
- Near nightlife venues.
- Limited competition for Italian restaurants.

## 2 Data acquisition and cleaning

## 2.1 Data Sources

We will use the Four Square API and its a data sources to obtain information on the overall areas the client is interested. In this case the downtown Toronto neighbourhoods. We will make use of the venue categories to narrow our search criterea. The following catgeories will be used:

- Food
- Italian Restaurant
- Nighlife Spot

The Food category will be used to obtain an overall idea of the number of restaurants in a given neighbourhood. The Italian Restaurant category will by used to determine if a neighbourhood already has a good selection to choose from.

We will merge the Nightlife and Restaurant location data to get an idea for a possible location.

We will also use the Wikipedia data on postal locations for the Toronto area to map the neigbourhoods actual location.

### 2.1.1 References

Links to information on the data sources used:

[Foursquare Search Endpoint Details](https://developer.foursquare.com/docs/api-reference/venues/search/)

[Foursquare Venue Categories](https://developer.foursquare.com/docs/build-with-foursquare/categories/)

[Wikipedia Toronto Postal Codes](https://en.wikipedia.org/wiki/List_of_postal_codes_of_Canada:_M)

### 2.2 Data Cleaning

We will narrow the search from the Toronto area to the downtown area only. We will also throw out any P.O. Box locations as this is not a real neighbourhood.

We will also clean up some of the Italian Restaurants. Included in the search were Italian bakeries and Pizza places which are not the type of restaurant the client is looking to open so these will be dropped.
