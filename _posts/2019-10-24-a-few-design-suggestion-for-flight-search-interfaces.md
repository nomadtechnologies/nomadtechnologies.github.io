---
layout: post
title: A Few Design Suggestions For Flight Search Interfaces
date: 2019-10-24 01:38
categories:
author: Afra Melia
---

This article investigates ways in which booking interfaces can be improved. In this particular project we choose to focus on flight booking interfaces.
 <!-- It helps to find a cheaper flight after choosing different dates on the calendar, giving a better view of rates and dates. This modification is made for this people who are looking for cheap flight without having to look day per day, something that is very long and tedious, ending up with frustrating user specially if he found that is he had choose other dates the flight could have been lot more cheaper. -->

## The Problem
Imagine a situation in which you are looking to take a short holiday or planning to visit family abroad and want to book a flight. You want the flight to be cheap and you're quite flexible with dates. You go to look for tickets on the relevant website (e.g. Skyscanner or Ryanair) and start looking for a flight. For the days you specify the website retrieves tickets that are way beyond your budget, so you go back to enter in new dates and continue this process indefinitely until you manage to find your ticket.
This process is clearly tedious and frustrating! What we propose below is an attempt to remedy some of these issues.

## The Solution
The solution is simple. We propose allowing the user to specify a range of possible dates as well as a minimum and maximum budget and then retrieving a sorted list of tickets within the date range. We also allow the user to view these tickets via a calendar grid. In summary this enables the user to view all of the prices without having to search day by day.

## Interviews
The first step was interviewing some regular flight search users. In this case I interviewed three people aged between 20-30.
Few things that they had in common was the love of travel as well as having family abroad they liked to visit regularly. They normally look for cheap flights and better still if they manage to secure direct flights with a well-known airline carrier. Something else that I have noticed is that they look for flights months in advance in an attempt to get cheaper flights especially if they intend to travel during the holiday seasons.

So I picked some important goals for the user and sorted them from most important to least important.
1.	Searching for the cheapest flight.
2.	Looking for best dates to fly.
3.	Being able to set a budget in the search engines.
4.	Not to have to do the calculations (having a clear results of the total flight cost and date).
5.	To get just the known and trusted companies.
6.	No changing on cost when selected the flight.
7.	To do the booking easy and quick.

## Personas
After the interviews I was able to create a user persona.

![pic](/assets/images/personas.png){: width="300px"}

## Wireframes
The first step I took to create the app was to draw some wireframes.
Once I was happy with the wireframes I asked for feedback before starting with the prototype, this way it means
I can fix the wireframe and not to wait until the prototype in case of an error.
The final wireframe:

![pic](/assets/images/search.jpeg){:height="500px" width="300px"} ![pic](/assets/images/calendar.jpg){:height="500px" width="300px"}

## Prototype
Once the wireframes were done I started with the prototype of the final product that will look like these.

![pic](/assets/images/flight-search.gif){: .center-image }

On the image we can see that once you input all the data, like the early day you are willing to travel and the latest day you want to come back and the days you are going to be away, the app looks for the cheapest flight and it shows the days on the calendar. If you scroll down you can see the other options and if you click on them it shows the days on the calendar.
You just have to choose the one that suits you best.

## Features
At the end we have a flight search interface that the user just have to fill in the information required like destination, budget they are able to spend and the days the user will travel, the app will look for the best flight taking in count all the user requirements.
It will show a scrolling option where the first option will be the cheaper as well as the option the see it on a calendar so he can have a better look of the options and choose the one that suits him best.
These way will be a lot more quicker and efficient since the user will not have to calculate the total amount of the flight cost, will be clear total amount without any extra surprises and will not miss any better option.
Once the user choses the flight we added and option of making a picture of the passport so the user don't have to go through the pain of filling all the boxes it will automatically be filled in and same with the payment method. These way will be quicker and secure because will not have to worry about making any mistake that might be charged if you want to rectify it later like a lot of companies do.

## Summary
This project started as an assignment taken from The Gymnasium online UX course (url) but when I conducted the interviews I realised that it was an important matter for a lot of users so I decided to do undertake it as a real first UX personal project. The challenges I found were mainly around was fitting all of the search results neatly into a single viewport. I chose to go with the calendar format because it is most familiar to most users. In summary I would wish to see this feature implemented on a lot of sites as I think it would be a great time-saver.
