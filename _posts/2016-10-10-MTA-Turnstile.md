---
layout: post
title: Project Benson
---

This was the very first project at the Metis Data Science Bootcamp.  The purpose of the project was to analyze MTA turnstile 
data giving the number of entries and exists through each turnstile in the MTA subway system over a three month period.  
Counts at each turnstile are recorded in a cumulative manner and data is recorded approximately every four hours.

The goal of the project is to assist an organization hosting a summer gala.  The organization wants to deploy teams to 
various subway stations to get email addresses from as many people as possible.  The organization will then send tickets 
to these people via their email address in the hopes that they attend the gala.

We downloaded the data as a csv file, used Pandas to read the csv and convert it to a Pandas dataframe.  Furthermore, we cleaned 
the data by discarding counts that are negative (you can't have a negative amount of people entering or exiting through a turnstile), as well as
counts that are greater than around 10,000 -- which is roughly the number of seconds in four hours (you cannot realistically expect 
to have more than one person go through a turnstile per second).  We also subtracted consecutive entries and consecutive exits, then added these 
differences to obtain the number of people entering and exiting each turnstile during each four hour period.  Finally, we added together 
the counts and exits to obtain the total traffic through each turnstile during each four hour period.

From there, we can find total daily traffic, total traffic on weekdays versus weekends, and we can rank the stations by their total traffic.

More to come soon.  I will add graphs and describe our conclusions!  Stay tuned...


![alt text](https://github.com/unif2/unif2.github.io/blob/master/images/Benson.jpg)