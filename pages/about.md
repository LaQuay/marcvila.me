---
layout: page
title: About Me
permalink: /about/
weight: 5
---

# **About Me**

Hi!:wave: I am **{{ site.author.name }}**,<br>
Computer Science Engineer based in Barcelona. <br>
Industrial Ph.D. student in Computer Science at <a href='https://www.upc.edu'
target='_blank'>Universitat Politècnica de Catalunya</a> and working at <a
href='https://www.worldsensing.com/' target='_blank'>Worldsensing</a>. <br>
If you are interested in working with me or anything similar, feel free to get in touch.

<div class="row">
{% include about/skills.html title="Programming Skills" source=site.data.programming-skills %}
{% include about/skills.html title="Other Skills" source=site.data.other-skills %}
</div>
And other technologies / frameworks / tools, such as: Java, Javascript, Flask, Angular, Nginx, 
InfluxDB, NodeJS, C++, C, Firebase, Grafana, SQL, HTML, XML, CSS, ...

# **Work Experience**

<div class="row">
{% include about/work_timeline.html %}
</div>

# **Education**

<div class="row">
{% include about/education_timeline.html %}
</div>
