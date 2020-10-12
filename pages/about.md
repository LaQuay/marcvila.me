---
layout: page
title: About
permalink: /about/
weight: 3
---

# **About Me**

Hi! I am **{{ site.author.name }}** :wave:,<br>
A Computer Science Engineer based in Barcelona. Industrial Ph.D student in Computer Science at 
<a href='https://www.upc.edu' target='_blank'>Universitat Politècnica de Catalunya</a> and working at
<a href='https://www.worldsensing.com/' target='_blank'>Worlsensing</a>. If you are interested in working
with me or anything similar,  feel free to get in touch with me.

<div class="row">
{% include about/skills.html title="Programming Skills" source=site.data.programming-skills %}
{% include about/skills_no_perc.html title="Other Skills" source=site.data.other-skills %}
</div>
And many more, such as: Java, Nginx, InfluxDB, NodeJS, C++, C, SQL, HTML, XML, CSS, ...

# **Work Experience**
<div class="row">
{% include about/work_timeline.html %}
</div>

# **Education**
<div class="row">
{% include about/education_timeline.html %}
</div>
