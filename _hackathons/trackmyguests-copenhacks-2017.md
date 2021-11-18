---
name: TrackMyGuests
subtitle: Copenhacks 2017 - Denmark
tools: [Angular JS, Python, Flask, Leaflet, Twilio]
image: /assets/img/hackathons/copenhacks_2017/featured.png
description: Manage your local events with hosts and SMS services.
order_number: 5
---

# TrackMyGuests – CopenHacks 2017

April 2017 - Copenhagen (Denmark)

### The hackathon

Original event description:

> ... 24h of Hacking - Have you ever wanted to code a great idea but haven't been able to set aside
> the time to actually build it? Or perhaps you had a fantastic idea but lacked the technical
> ability to be able to code it yourself. Now you have the chance to dedicate 24 hours on this
> project or idea. The only condition is: You will only be judged on what you write within these 24
> hours. ...

> Hacking starts at 9:00 AM on Saturday and ends at 16:00 PM on Sunday.

### The solution

Imagine you have an event at home and you want to know where are your guests, and also remember them
not to arrive late. With a simple control panel, the host can manage this event and check which
guests are coming. When the host requires it, the system sends an SMS to the guests reminding them
about the meeting. This SMS activates an Android Service which sends the confirmation and the
guest's position to the host. That results are shown in a list and also in a map on the website.

- A frontend server in Angular 2, that shows the control panel to the hosts.
- A backend server API in Flask, that also uses the Twilio API to send the SMS.
- An Android native Application/Service to send the host the required information.

<img src="/assets/img/hackathons/copenhacks_2017/screen1.png" width="800"/>
<br>

<div style="text-align: center;">
<img style="margin: 0 !important; float: left" src="/assets/img/hackathons/copenhacks_2017/screen2.png" width="500"/>
<img style="margin: 0 !important; display: inline" src="/assets/img/hackathons/copenhacks_2017/screen3.jpg" width="280"/>
</div>
<br>

#### Languages

- Angular JS
- HTML
- CSS
- Flask
- Python

#### Technologies

- Leaflet
- Twilio

#### Team

- Francesc De Puig
- Ester Lorente
- Marc Vila

Hackathon result: -.

Role in the project: Angular 2 developer, frontend. And helping with the backend side.

Project code: [TrackMyGuests - GitHub](https://github.com/elorenteg/copenhacks17).

Appears in:

- [TrackMyGuests - Devpost](https://devpost.com/software/trackmyguests/)

Hackathon website: [CopenHacks at Devpost](https://copenhacks.devpost.com/).
