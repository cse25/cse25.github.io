---
layout: page
title: Projects
subtitle:
---

# News Aggregator

**Get the latest news articles from 60 sources**

I created a news aggregator as a chance to learn more about the React ecosystem and to create a simple way to browse the day's news all in one place. Users can access the news dashboard without signing in or signing up. Alternativey, they may make an account to save their favorite news sources to their dashboard for faster reference.

![Dashboard](/img/dashboard.png)
*News Dashboard*

To handle authentication I used bcrypt to hash and salt passwords, JSON web tokens to verify authenticated users, and passport as authentication middleware. I used MongoDB to store my data and Mongoose to work with my data.

![Favorites](/img/news-aggregator-favorites.png)
*Favorites*

Tech Stack: React, Redux, Node, Express, MongoDB

[GitHub](https://github.com/cse25/news-aggregator) | January 2017

---

# Forcefield

**Campus security solution consisting of hardware button, mobile and web apps**

![Forcefield Logo](/img/forcefield-iphone.png)

With Forcefield, my team and I set out to develop an alternative to the emergency poles commonly seen dotting the landscape of college campuses.  Forcefield would allow campuses to uphold student safety while eliminating the need to install and maintain costly emergency poles.  We decided to create an app that would allow students to alert campus security of their location utilizing their smartphone's built in GPS.

![V.BTTN](/img/button.png)

We built Forcefield around the [V.BTTN](http://www.vsnmobil.com/products/v-bttn-wearable-bluetooth-le-4-0-device), a wearable Bluetooth Low Energy device.  The user registers with our app by selecting their school or other institution, and then inputs their contact information.  The button is then paired with the app by holding the button down for eight seconds.  Once paired, the app quietly runs in the background.  When the user feels they are in danger, they simply press the button.  The smartphone then transmits the user's location with web sockets, as well as database queries for record keeping.  The user's name, phone number, emergency start time, emergency end time (if applicable), as well as location are rendered on the officer dashboard.  At this point the security officer can phone the student to check if they are safe, or dispatch a nearby officer to the emergency location.  The location updates on the dashboard every few seconds, and a trail is generated to show where the student has been.  The officer may also set resolved emergencies inactive as well as view a heat map of previous emergencies.

![Forcefield Dashboard](/img/forcefield-dashboard.png)
*Security Officer Dashboard*

What sets Forcefield apart from other personal safety apps is having easy access to your application through the hardware button.  In the case of other apps, having to unlock your smartphone, open your app and touch the screen can feel like an eternity when you're in danger.

Tech Stack: Angular, Ionic, Node/Express, MySQL, Socket.io

[GitHub](https://github.com/MKS-Elixr/forcefield) | May 2016

---

# Notesee

**Mobile application for classroom note sharing and collaboration** 

![Notesee Logo](/img/notesee-banner.png)

My team and I decided to create a mobile application for students to share and organize their classroom notes.  The basics: a student signs into our app, creates a classroom, shares the join code with classmates and they post notes to the classroom.  They post these notes by taking pictures with their smartphone camera and pressing 'upload.'  Stretch goals included: a tagging system for filtering notes by topic, an upvote and downvote feature, optical character recognition (OCR) and note annotation. 

We deployed our app to an AWS EC2 instance running Ubuntu and used Amazon's S3 to store our images.  We decided to convert our images to base64 strings and store the URL returned from S3 so we could get better performance and not store large images in our database directly.

In the end, we ran out of time before implementing our stretch goals but were satisfied with our final product.  It met all of our requirements for basic functionality and looked and felt polished.

Tech Stack: Angular, Ionic, MySQL, AWS, S3

[GitHub](https://github.com/MKS-PostgreSQL/notesee) | April 2016

---

# Open2

**Web application for scheduling last minute events with friends**

The premise for this app was for my team to inherit a legacy codebase from another group.  We were asked to make improvements under a three to four day time constraint. Speaking with the team that produced the app gave us the opportunity to find out what features they would have liked to see added. Afer this intitial consultation period, we were not permitted to ask them further questions for the duration of the project.

We chose to inherit Open2 because we saw a lot of potential to enhance the user experience in this social media platform.  The original app functioned by having users post an activity along with a date and time which would get broadcast to select friends.  Users in the network could then RSVP with a single click.  That being said, the app felt a bit limited since it lacked a chat feature. Feeling that one was pretty essential, we decided it was a priority to implement.  The chat we added functioned similarly to a group text and was accomplished with Angular, Socket.io, and MySQL.  In addition, we added a map displaying the live location of users.  Lastly, we significantly refactored their HTML and JavaScript to abide by JS Standard.

![Open2 Dashboard](/img/open2-dashboard.png)
*Open2 Dashboard*

Tech Stack: Angular, MySQL, Node/Express, Socket.io

[GitHub](https://github.com/MKS-PostgreSQL/open2) | April 2016

---

# FourSquare Photo Explorer

**Web application for viewing FourSquare users' photos**

I built this single page app to for a coding challenge whose requirement was to use Angular to make a request to a social API and display the results on the page.  The user enters a term in the search bar and is presented with the top ten results in Los Angeles. Clicking on a result displays a gallery of photos from FourSquare users.

![FourSquare Photo Explorer Dashboard](/img/foursquare-explorer.png)
*FourSquare Photo Explorer Dashboard*

Tech Stack: Angular, Bootstrap

[GitHub](https://github.com/cse25/foursquare-photo-explorer) | July 2016

---

# Trade Apprentice

**Web application to simulate stock trading and track portfolio over time**

I created Trade Apprentice under a 36 hour time constraint as part of our MVP (Minimum Viable Product) Project.  This was our first project at MakerSquare after working through six weeks of 2-3 day sprints.  I built Trade Apprentice independently, which exposed me to iterative development methods.

I designed a platform to allow hobbyist day traders to make "paper trades," i.e. simulated trades having no financial risk.  The user enters an amount of their choice to deposit in their account, click 'deposit,' and then they're ready to trade.  Entering a valid stock symbol will provide up-to-date information on the specific stock.  The user can then buy or sell shares and have the balance of shares be reflected in their portfolio.  Clicking 'Refresh Portfolio' pings the API once for each entry in their portfolio and then updates the page with the latest price. 

![Trade Apprentice Screenshot](/img/trade-apprentice-screenshot.png)
*Trade Apprentice Dashboard*

I quickly styled the app with the CSS framework Materialize to make it look presentable.  There are some features I would have loved to have implemented if time permitted.  For starters, having the possibility for the creation of user accounts and persisting data would be a top priority.  A graph showing performance over time would be a close second.  Another means of improvement would be making the app competitive. For example, users could compete to see who can make the most money by trading in a fixed number of weeks.  In the end, making the app demo ready was my first priority. Since this project, I have had plenty of opportunities to improve my Angular skills.

Tech Stack: Angular, Node/Express, MarkIt API, Materialize

[GitHub](https://github.com/cse25/trade-apprentice) | April 2016

---
