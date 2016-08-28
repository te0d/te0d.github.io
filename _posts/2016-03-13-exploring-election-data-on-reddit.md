---
layout: post
published: false
title: Exploring 2016 Election Data on Reddit
category: Blog
tags:
  - Reddit
  - Data
  - Politics
---

I was browsing reddit when I noticed that the subreddits /r/SandersForPresident and /r/The_Donald both had links on the All front page. This got me thinking that maybe there could be some interesting correlations of the users of both of these subreddits. I'm interested in the language used in comments on candidate specific subreddits. Also, I'm interested in the other subreddits commented on by users who comment on candidate specific subreddits. And if there's time, I'll try to look at relations between users and state-specific subreddits, as well as the comments of state specific subreddits.

Getting the Data
================

While it's possible to grab data from reddit by appending *.json* to a page's URL, I will be using the official reddit API. Looking at the rules, I see that 60 requests are allowed per minute. I will be grabbing the past 6 months of links from the subreddits /r/SandersForPresident and /r/TheDonald. In addition, I will be grabbing the past 6 months worth of comments made by a subset of users from each subreddit.

To retrieve the data, I have written a ruby script which uses the Redd gem to wrap the API. I then put this data into a postgresql database. Before we can access the reddit API, we need to get a client id and secret token. We do this by going to your user's preferences and then switching to the apps tab. There we can create a new application which will be assigned the necessary client id and secret key.

To get the first 6 months of data on a subreddit, we will be using /subreddits/new to loop through pages of posts until we reach the desired time.
