---
name: Neighborgood
subtitle: HackUPC 2018 - Spain
tools: [React, Serverless, DynamoDB, Lambda]
image: /assets/img/hackathons/hackupc_2018/featured.png
description:
   Web-app that compares the different neighborhoods of Barcelona based on different criteria (environment, economic, population, security).
order_number: 16
---

# Neighborgood – HackUPC 2018

October 2018 - Barcelona (Spain)

### The hackathon

Original description from the organizers [HackUPC at Devpost](https://hackupc2018.devpost.com/):

> BarcelonaTech student Hackathon. 700 hackers. 36 hours. Dream it. Hack it. Ship it.

> Hacking starts at 22:00 PM on Saturday and ends at 13:00 PM on Sunday.

### The solution

We love social projects and we wanted to create one that would have a positive impact on the community. Recently some members of the team have had to look for a rental apartment in Barcelona, one of the main problems of the city. We realized the difficulty of renting a house in good condition for a fair price.

For us it was difficult to know if a flat really was worth it not only taking into account the state of the house but also the area where it is located. What is the neighborhood that best suits our lifestyle? What is the real value of a house taking into account the services, environmental conditions and the type of population that lives in it?

All these questions were not answered in the usual rental portals such as Idealista, Fotocasa or Habitaclia and we wanted to answer them by ourselves and make this data accessible to everyone.

<div style="text-align: center;">
<img style="margin: 0 !important; float: left" src="/assets/img/hackathons/hackupc_2018/screen1.jpg" width="430"/>
<img style="margin: 0 !important; display: inline" src="/assets/img/hackathons/hackupc_2018/screen2.jpg" width="430"/>
</div>

Neighborgood is a web-app that compares the different neighborhoods of Barcelona and surroundings areas based on several criteria such as environmental (air quality, number of trees and green areas), economic (average rental price), population (number of tourist apartments) or security.

It is a service that aims to quantify the level of wellbeing of each area and so that any person can choose the place where they live, work, create a business or educate their children in a free and informed way.

All these data are shown on the web-app as heat maps where the best results are shown in green tones and the worst ones go from yellow to red as they get worse.

We use the data that Barcelona Open Data offers as source of information. This information is stored inside a Amazon DynamoDB, which is accessed through Amazon Lambda and the Amazon API Gateway. Then the information is displayed in a React, which is inside an Amazon EC2. But all the backend is “serverless”.

#### Languages

- React
- Spring
- Python

#### Technologies

- Amazon DynamoDB
- Amazon Lambda
- Amazon API Gateway
- Barcelona Open Data
- LeafletJS

#### Team

- Ester Lorente
- Sandra Martín
- Juan Salmerón
- Marc Vila

Role in the project: Backend.

Project code: [Neighborgood - GitHub](https://github.com/elorenteg/HackUPC2018).

Appears in:

- [Winner HackUPC Winter 2018 - AWSEducate challenge](https://devpost.com/software/neighborgood)

- [Winner HackUPC Winter 2018 - Bloomberg challenge](https://devpost.com/software/neighborgood)

Hackathon website: [HackUPC 2018](https://2018.hackupc.com/).
