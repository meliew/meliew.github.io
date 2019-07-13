---
layout: post
title:      "Creating my first CLI program"
date:       2019-07-12 21:50:52 -0400
permalink:  creating_my_first_cli_program_-_mystery_cli
---

#Mystery CLI 


When I first saw the instructions for our CLI project, I thought, “well, this probably won’t be too hard.” It wasn’t long before I changed my mind. 

Up until this point in the program we’ve had our training wheels on - we get labs with tests, so we know exactly what we’re supposed to do, and often how to fix it when it goes wrong. 

This time, we were on our own, and let me say - it wasn’t easy. 

For my project, I decided to scrape the Goodreads website to get a list of mystery sub-genres. Why mystery? Well, as a mystery reader (and someone who dabbles in a bit of mystery writing) I thought it would be a project that would keep me interested and would actually be useful for me as I look for new books. The great thing about this project is that while it is currently setup to only scrape for mystery subgenres, it can easily be expanded to scrape for other categories as well. 

The first thing I did when starting out was create my scrapers. I had originally started this project with another website and instantly found that the scrapers would give me trouble, so I wanted to make sure upfront that I’d be good to go. The way the scrapers work are they scrape a general mystery page to get names and URLs for all the subgenres, and then it scrapes each of the subgenre URLs for a bio and a list of new releases (which updates regularly). 

Getting the scrapers working was quite a task. I was able to get the first level scraper up and running fairly quickly because it was straight forward. For the second level scraper, I had to take quite a bit of time in order to get the right selectors, and then I had to be sure to scrape only the information I wanted. This was difficult because the class that was used for the new release titles was also used to list popular titles on another portion of the website. It wasn’t until I found the container for the new releases and paired that with the class that I was able to get those titles scraped. 

Once the scrapers were working as they should, and creating new instances of the Genre class, it was time to get started on the CLI class. 

The CLI interface was straightforward to put together, although not without its challenges. I started with an intro method that welcomed users to the program, then gave them a list of subgenres (scraped info) to choose from. After a user selects a subgenre they will see a bio/description. Next, the user is asked if they’d like to see a list of new releases or go back to select a new subgenre. 

I think one of the hardest parts of creating the CLI portion was looping the user back to the beginning without re-scraping. This issue was solved by storing all info for each instance of the Genre class in an array. 

There were times during this program when I really didn’t think I’d be able to complete it - and then other times when I felt like I was really doing well. I even found that I had time at the end to add some fun and flair to my program by using colorize to break up the sections of text and give it a more personal feel. 

I also think I learned more during these two project weeks than at any other time in the program. While I don’t feel like an OOP Ruby expert by any means, I think at this point I’d be able to build another simple CLI project and I would not have been able to say that two weeks ago. I’m excited to see what we learn next! 


