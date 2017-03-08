---
title: "Hackbright Project: Eat Together"
layout: post
date: 2017-01-03 08:00
image: /assets/images/profile.jpg
headerImage: false
projects: true
blog: false
tag:
- hackbright
- project
- python
author: michellekim
description: Hackbright project description
---

![](../assets/images/proj-et/et1.gif)

## Summary:

This was my project at Hackbright Academy, spanning 4 weeks during the Software Engineering Fellowship.

#### About Eat Together

Eat Together helps two people decide on a place to to share a meal together. Each user can input their locations and the types of restaurants they’d like to visit and search on Yelp according to both sets of preferences. The search results are then shown on a map with markers that provide more information about each business in the search results. Users can create accounts and keep track of visits, and Eat Together will provide a recommendation on which restaurant is ‘similar’ to their most highly rated restaurant.

#### Tech Stack
- Python
- JavaScript
- jQuery
- AJAX
- PostgreSQL
- SQLAlchemy
- Flask
- SciPy Libraries
- HTML
- CSS
- [Material Design for Bootstrap](http://fezvrasta.github.io/bootstrap-material-design/)

#### APIs used
- [Yelp](#https://www.yelp.com/developers/documentation/v3)
- [Google Maps Javascript](https://developers.google.com/maps/documentation/javascript/)
- [Google Places Javascript Library](https://developers.google.com/places/javascript/) - for the form's Autocomplete
- [Google Maps Distance Matrix](https://developers.google.com/maps/documentation/distance-matrix/intro)

---

## Updates
It's been [deployed to Heroku](https://eatog.herokuapp.com/), but it runs pretty slowly.  If, upon loading, the Google Map does not display, press `cmd+shift+r`.  I've put aside further development on Eat Together until after I progress further in my newer projects.

___

## GIFs
Filling out the form generates a list of search results from Yelp and generates markers on the Google Map
![](../assets/images/proj-et/et1.gif)

You can log a visit to a restaurant by rating it, recording the date of the visit, and saving it to your profile - which on the back-end, saves this information to the PostgreSQL database
![](../assets/images/proj-et/et2.gif)

The search results are dynamically-generated Yelp links, and the map markers are embedded with Yelp restaurant information
![](../assets/images/proj-et/et3.gif)

Your profile page shows a query on your username from the PostgreSQL database on all of your past visits, and uses a simple euclidean distance formula to calculate another restaurant in the database whose numeric data is most similar to your most recently highly rated restaurant
![](../assets/images/proj-et/et4.gif)

___

## Future planned improvements
- Groups of 3 or more can search for a location
- Use the K-nearest-neighbors algorithm to identify similar restaurants that the user has not visited
- Add functionality to the table to allow filtering of past visit view by person user visited with, date, rating
- Add graphics on top of the map to visualize the midpoint formula and venn diagram methods of searching for a good location to meet up.
