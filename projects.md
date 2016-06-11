---
layout: page
title: Projects
subtitle: Here are some of my more recent projects.
---

# Forcefield

**Campus security solution consisting of hardware button, mobile, and web apps**

>![Forcefield Logo](/img/forcefield-iphone.png)
_Forcefield Splash Page_

When brainstorming ideas for an app, we wanted to try to improve the emergency poles commonly seen dotting the landscape of college campuses.  Since research shows these beacons are mostly ineffective at preventing abduction, as well as costly to install and maintain, we decided to create an app that would allow students to alert campus security of their location using their phone's GPS.

>![V.BTTN](/img/button.png)
_V.BTTN Hardware Button_

We built our app around the [V.BTTN](http://www.vsnmobil.com/products/v-bttn-wearable-bluetooth-le-4-0-device), a wearable bluetooth low energy device.  The user registers with the app by selecting their school or institution and the button is paired with the app on the user's smartphone by holding the button for eight seconds.  After pairing, the app runs in the background and waits for a button press.  When the user feels they are in danger, they simply press the button.  The smartphone then transmits the user's location with web sockets, as well as database queries for record keeping.  The users' name, phone number, emergency start date and time, emergency end date and time (if applicable), as well as location updated every few seconds, are shown on the dashboard.

>![Forcefield Dashboard](/img/forcefield-dashboard.png)
_Security Officer Dashboard_

[Click Here](http://forcefield.herokuapp.com/#/dashboard) to give the dashboard a try.  I've put some fake emergencies in our database for demonstration purposes.

Our tech stack:
* Angular
* Ionic
* Node/Express
* MySQL
* Socket.io

[GitHub](https://github.com/MKS-Elixr/forcefield) | May 2016

---

# Notesee

**Mobile application for classroom note sharing and collaboration** 

...Content Coming Soon...

>![Notesee Logo](/img/notesee-banner.png)

_Notesee Logo_

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
