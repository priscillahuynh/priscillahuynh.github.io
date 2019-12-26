---
layout: post
title:      "Sinatra Portfolio Project"
date:       2019-12-26 05:12:25 +0000
permalink:  sinatra_portfolio_project
---

Before I began coding this project, I knew the single most important task would be to clearly map out the object relationships first. However at the same time, I got really excited to create something unique and useful. Even after carefully considering my models and relationships before starting, I still ended up over complicating it and tossed the project after two days. I needed to think more simply. 

My second version is much simpler and completely different. Its a basic goal tracking app that lets a user log in, create a goal with a title and description, and edit or delete it if needed. 

There are only two models, a Users and a Goals class. At its current state it's definitely too simple for my liking, but I have a lot of ideas on how to expand upon it later. Some of the features I hope to add in the future include:

1. Daily entries that are written first thing in the morning and at the end of the day. Each morning entry describes ONE thing that the user can do today that will bring them one step closer to their goal. And each evening entry would allow the user to click one of  two buttons - did they accomplish that task? Or did they let their excuses take over? If so, then they need to write down their excuse that day.
2. Each morning entry will be formatted to be as specific and concise as possible. "I will [ACTION] at [TIME] in [LOCATION]"
3. Excuses will be displayed along a side panel for the user to see every day.
4. Every consecutive day of a completed task will be marked with an X on the calendar to show any positive streaks.
5. Display a new motivational quote for the user to see every day. 

I also wanted to incorporate validation failures to the user using the rack-flash gem but could not get it to work for the life of me. This is definitely be something I would hope to cover during my project review. 

I should also add that the single greatest resource I had that helped me complete this project were the "Sinatra Live Build Journal App" videos found here[https://instruction.learn.co/student/video_lectures#/?query=journal](http://). There are 9 videos total, and each about an hour long. Howard's walkthrough and explanations were extremely helpful to not only complete this project but also to gain a solid understanding of how every line of code works.

I have many more ideas on how I'd like to expand on this project. However for the sake of my sanity and to maintain a good speed of progression in this course, I figure done is better than perfect. 


