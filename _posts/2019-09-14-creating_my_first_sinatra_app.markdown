---
layout: post
title:      "Creating My First Sinatra App "
date:       2019-09-15 03:40:06 +0000
permalink:  creating_my_first_sinatra_app
---


It took me a while to figure out what I would choose for my Sinatra project, but I finally landed on an idea - a code challenge tracker. I was excited to dive in and try my hand at creating my own MVC app, and it was a fun project, yet also full of challenges (just what you’d expect, right?). 

To get started, I took my instructor’s advice to start with what I knew how to do, so that meant creating the Models. From there I created my database, then started creating my controllers. When we first learned about separating controllers I was a little concerned that it would make my life harder. I mean, you have to have separate controllers for EVERY model? But, the reality is, this format makes life a whole lot easier. Why? Well, for starters, when you need to find a route, there isn't an endless chain of scrolling, or searching for terms in the code. It’s straightforward and easy to find. You’re looking for the signup route? Great, look in users_controller. You’re looking to delete a post? You’ll find that in the posts_controller. 

# My app layout 

My app is fairly simple, but I have plans to add to it as time goes on. The way it works now is a user will signup for an account by selecting a username and password, and also supplying their email address. If they select a username that has already been taken, a friendly flash message will let them know. Once they login, the user can create challenges, view their challenges, and also edit or delete their challenges. The functionality additions that will come down the line include a countdown for the days of the challenge, plus a way to update a log by date. I also plan to include functionality that lets users comment on each other’s challenges. 

For now, the user, once logged in has the choice to view all their own challenges, view a specific challenge that belongs to another user, edit their own challenges, delete their own challenges, or create a new one. It’s a simple app with a lot of possibilities.
# A challenge in the challenges_controller

One challenge I ran into as I was working through this app was that while I had created a 404 page that would show up whenever a user tried to go to a non-existent page, there was one type of error that didn’t display this page. If a user tried to go to a route such as /challenges/29342 and say that number did not exist, it was redirecting to a different route rather than the 404 page. 

To fix this, I had to make a few changes to the logic. First, we’d check to see if someone was logged in. If not, they would get re-routed to the login page. Next,  I checked for the challenge by ID. If there was a challenge by that ID number it would show the page. If there was no challenge with that ID, then I called the not_found method, which displayed the 404 page view. 

# Things I’ve learned

I learned a lot going through the process of creating this app. One thing I learned was how much I still have to learn. I also learned that I’ve learned a lot. (Try saying that 10 times fast). 

All kidding aside, I think the skills of learning how to find the answers I need, learning how to ask the right questions, and learning how to read code have been made so much stronger thanks to this project. 

I look forward to moving on to Rails and seeing what else I can do! 




