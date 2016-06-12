---
layout: page
title: Projects
subtitle: Here are some of my more recent projects.
---

# Forcefield

**Campus security solution consisting of hardware button, mobile and web apps**

>![Forcefield Logo](/img/forcefield-iphone.png)

With Forcefield, my team and I set out to develop an alternative to the emergency poles commonly seen dotting the landscape of college campuses.  Research shows these beacons are mostly ineffective at preventing abduction, as well as being costly to install and maintain, so we decided to create an app that would allow students to alert campus security of their location utilizing their smartphone's built in GPS.

>![V.BTTN](/img/button.png)

We built Forcefield around the [V.BTTN](http://www.vsnmobil.com/products/v-bttn-wearable-bluetooth-le-4-0-device), a wearable Bluetooth Low Energy device.  The user registers by selecting their school or other institution and then inputs their contact information.  The button is then paired with the app by holding the button down for eight seconds.  Once paired, the app quietly runs in the background.  When the user feels they are in danger, they simply press the button.  The smartphone then transmits the user's location with web sockets, as well as database queries for record keeping.  The users' name, phone number, emergency start time, emergency end time (if applicable), as well as location are rendered on the officer dashboard.  At this point the security officer can phone the student to check if they are safe, or dispatch a nearby officer to the emergency location.  The location updates on the dashboard every few seconds, as well as a trail showing where the student has been.  The officer may also set resolved emergencies inactive as well as view a heat map of previous emergencies.

>![Forcefield Dashboard](/img/forcefield-dashboard.png)
*Security Officer Dashboard*

[Click Here](http://forcefield.herokuapp.com/#/dashboard) to give the dashboard a try.  I've inserted some fake emergencies in our database for demonstration purposes.

What sets Forcefield apart from other personal safety apps is having easy access to your application through the hardware button.  In the case of other apps, having to unlock your smartphone, open your app, and touch the screen can feel like an eternity when you're in danger.

Tech Stack: Angular, Ionic, Node/Express, MySQL, Socket.io

[GitHub](https://github.com/MKS-Elixr/forcefield) | May 2016

---

# Notesee

**Mobile application for classroom note sharing and collaboration** 

>![Notesee Logo](/img/notesee-banner.png)

My team and I decided to create a mobile application for students to share and organize their classroom notes.  One of the first things we discussed as a team was what we wanted our app to do at a high level.  The basics: A student signs into our app, creates a classroom, shares the join code with classmates, and they post notes to the classroom.  They post these notes by taking pictures with their smartphone camera and pressing upload in the app.  Stretch goals included: a tagging system for filtering notes by topic, upvotes and downvotes, optical character recognition (OCR), note annotation, and public/private classrooms. 

We deployed our app to an AWS EC2 instance running Ubuntu and used Amazon's S3 to store our images.  We decided to convert our images to base64 strings and store the URL returned from S3 so we could get better performance and not store large images in our database directly.

In the end, we ran out of time to implement our stretch goals but were satisfied with our final product, as it met all of our requirements for basic functionality and looked and felt polished.

Screenshots coming soon!

Tech Stack: Angular, Ionic, MySQL, AWS, S3

[GitHub](https://github.com/MKS-PostgreSQL/notesee) | April 2016

---

# Open2

**Web application for scheduling last minute events with friends**

The premise for this app was that my team inherit a legacy codebase from another group and be tasked with making improvements under a three to four day time constraint.  We had the opportunity to speak with the project's team prior to adopting their project to find out what features they would have liked to seen added, and gather any other pertenent information.  We were not permitted to ask them further questions after the allotted time.

We chose Open2 because we saw a lot of potential to enhance the user experience in this social media platform.  The original app functioned by having users post an activity along with a date and time which would get broadcast to your circle of friends.  Users in your network could then RSVP with a single click.  That being said, the app felt a bit limited so a chat feature was pretty essential.  The chat we implemented functioned similarly to a group text and was accomplished with Angular, Socket.io, and MySQL.  In addition, we also significantly refactored their HTML and Angular code to abide by John Papa's style guide.

Tech Stack: Angular, MySQL, Node/Express, Socket.io

[GitHub](https://github.com/MKS-PostgreSQL/open2) | April 2016

---

# Trade Apprentice

**Web application to simulate stock trading and track portfolio over time**

Trade Apprentice was an app I created under a 36 hour time constraint as part of our MVP (Minimum Viable Product) Project.  This was our first project at MakerSquare, after six weeks of 2-3 day sprints.  The idea was to see, as individuals, what the coolest thing we could build in under 36 hours, as well as expose us to iterative development methods.  

I built a platform to allow hobbyist day traders to make "paper trades", ie simulated trades having no financial risk.  The user enters an amount to deposit in their account, click deposit, and then they're ready to trade!  Entering a valid stock symbol will provide up to date information on the stock.  You can then buy or sell shares and have the balance of shares be reflected in your portfolio.  Clicking "Refresh Portfolio" pings the API once for each entry in your portfolio and then updates the page with the latest price. 

>![Trade Apprentice Screenshot](/img/trade-apprentice-screenshot.png)
*Trade Apprentice Dashboard*

I quickly styled the app with the CSS framework Materialize to make it look presentable.  There are some features I would have loved to have implemented if time permitted.  For starters, having user accounts and persisting data would be a top priority.  A graph showing performance over time would be a close second.  Another direction one could take it would be making the app a competition over who can make the most money by trading in a fixed number of weeks.  In the end, making the app work was the first priority and I have had plenty of opportunities since to improve my Angular skills.

Tech Stack: Angular, Node/Express, MarkIt API, Materialize

[GitHub](https://github.com/cse25/trade-apprentice) | April 2016

---
