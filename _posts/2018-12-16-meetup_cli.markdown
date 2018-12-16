---
layout: post
title:      "Meetup CLI "
date:       2018-12-16 01:25:12 -0500
permalink:  meetup_cli
---


### Tech Meetups in Los Angeles

I have always found Meetup groups to be a great opportunity to meet other people. And given the fact that I am making a complete career change into this field, I couldn't think of a better first project than a Tech Meetup CLI. 

Once the program starts, users are provided a list of 100 tech meetup groups in the greater Los Angeles area. They are prompted to make a selection and are then provided a summary of what that meetup is about. Topics range from programming languages, hackathons, cryptocurrency, AI and more.

After selecting and viewing the meetup group details, the program then provides the option to either view future events, or to return to the main menu. If the user selects "events", they are then provided the name, date, time, and description of the next event. 
 
### Classes
**1. Meetup Class** - Objects in this class are initialized with a meetup name, # of members, and the url for the specific meetup. Every object that is created is then added to a meetup array. The array is accessible via the #self.all method.

**2. Event Class** - If a meetup has an event scheduled for a future date, a new event object will be initialized with the meetup details. This includes the name, date_and_time, and event_description.

**3. Scraper Class** - There are 3 different methods in this class:
*  self.scrape_tech_meetups - this method scrapes the index page for tech meetups in Los Angeles and finds the values for the name, members, and url variables. It then creates a new meetup object by passing in those values.

*  self.scrape_meetup_page(url) - this method scrapes the url of each individual meetup group and provides details about what that meetup is about.

* self.scrape_meetup_event(url) - this method scrapes the url of each meetup and determines whether or not a future event is scheduled. If an event is scheduled, it will find the values for the name, date, time, and description of that event.

**4. CLI Class** - Interacts with the user prompting input and displays details about each meetup selected.

### Things I've Learned

**Patience & Persistence**
I felt so lost when I initially started this project. But several video tutorials and google searches later, I slowly started putting the pieces together. Instead of being frustrated with myself for not understanding something, I gave myself the time and opportunity to dive deeper into topics that didn't quite sink in initially.

**Binding.pry**
I had never fully understood how to use pry up until this assignment. I would watch several video tutorials and read documentation but nothing and no one has given me more clarity on the topic than this project. Learning how to use it made coding this CLI so much more fun! 

**Github Practice**
Just like pry, I developed a much greater understanding of how to interact with GitHub through this assignment.

**Understanding the working environment**
Honestly it sounds simple.....and it is, but prior to this project I had practically zero understanding of what files go where and which one does what. I just see it as taking another baby step in the right direction. There's a long road ahead but these small wins are what will help me reach that final goal! 

Being able to complete this project has been an incredibly uplifting and motivating experience. All of the lessons and topics that seemed fuzzy and unclear to me up until this point quickly began to make sense as I worked my way through this assignment.  While it is far from perfect, I am just really proud to have created my first fully functioning CLI from scratch. Looking forward to the projects lie ahead!
