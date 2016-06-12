---
layout: page
title: Projects
subtitle: Here are some of my more recent projects.
---

# Forcefield

**Campus security solution consisting of hardware button, mobile and web apps**

>![Forcefield Logo](/img/forcefield-iphone.png)

With Forcefield, we set out to develop an alternative to the emergency poles commonly seen dotting the landscape of college campuses.  Research shows these beacons are mostly ineffective at preventing abduction, as well as being costly to install and maintain, so we decided to create an app that would allow students to alert campus security of their location using their phone's GPS.

>![V.BTTN](/img/button.png)

We built Forcefield around the [V.BTTN](http://www.vsnmobil.com/products/v-bttn-wearable-bluetooth-le-4-0-device), a wearable Bluetooth Low Energy device.  The user registers by selecting their school or other institution, as well as inputting their contact information.  The button is then paired with the app by holding the button for eight seconds.  Once paired, the app quietly runs in the background.  When the user feels they are in danger, they simply press the button.  The smartphone then transmits the user's location with web sockets, as well as database queries for record keeping.  The users' name, phone number, emergency start time, emergency end time (if applicable), as well as location are rendered on the officer dashboard.  At this point the officer can phone the student to check if they are safe, or dispatch a nearby officer to the emergency location.  The location updates on the dashboard every few seconds.  The officer may also set resolved emergencies inactive as well as view a heat map of previous emergencies.

>![Forcefield Dashboard](/img/forcefield-dashboard.png)
*Security Officer Dashboard*

[Click Here](http://forcefield.herokuapp.com/#/dashboard) to give the dashboard a try.  I've put some fake emergencies in our database for demonstration purposes.

What sets Forcefield apart from other personal safety apps is having easy access to your application through the hardware button.  In the case of other apps, having to unlock your smartphone, open your app, and touch the screen can feel like an eternity when you're in danger.

Tech Stack: Angular, Ionic, Node/Express, MySQL, Socket.io

[GitHub](https://github.com/MKS-Elixr/forcefield) | May 2016

---

# Notesee

**Mobile application for classroom note sharing and collaboration** 

>![Notesee Logo](/img/notesee-banner.png)

We decided to create a mobile application for students to share and organize their classroom notes.  One of the first things we discussed as a team was what we wanted our app to do at a high level.  The basics: A student signs into our app, creates a classroom, shares the join code with classmates, and they post notes to the classroom.  They post these notes by taking pictures with their smartphone camera and pressing upload in the app.  Stretch goals included: a tagging system for filtering notes by topic, upvotes and downvotes, optical character recognition (OCR) integration, note annotation, and public/private classroom toggle.  

We deployed our app to an AWS EC2 instance running Ubuntu and used Amazon's S3 to store our images.  We decided to convert our images to base64 strings and store the URL returned from S3 so we could get faster performance and not store large images in our database directly.

In the end, we ran out of time to implement many of our stretch goals but were satisfied with our final product, as it met all of our basic requirements and looked and felt quite polished.

Screenshots coming soon!

Tech Stack: Angular, Ionic, MySQL, AWS, S3

[GitHub](https://github.com/MKS-PostgreSQL/notesee) | April 2016

---

# Open2

**Web application for scheduling last minute events with friends**

...Content Coming Soon...

[GitHub](https://github.com/MKS-PostgreSQL/open2) | April 2016

---

# Trade Apprentice

**Web application to simulate stock trading and track portfolio over time**

...Content Coming Soon...

>![Trade Apprentice Screenshot](/img/trade-apprentice-screenshot.png)

[GitHub](https://github.com/cse25/trade-apprentice) | April 2016

---
