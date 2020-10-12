---
layout: page
title: About
permalink: /about/
weight: 3
---

# **About Me**

Hi! I am **{{ site.author.name }}** :wave:,<br>
A Computer Science Engineer based in Barcelona.

# **Work Experience**
<div class="row">
{% include about/work_timeline.html %}
</div>

# **Education**
<div class="row">
{% include about/education_timeline.html %}
</div>

<div class="row">
{% include about/skills.html title="Programming Skills" source=site.data.programming-skills %}
{% include about/skills.html title="Other Skills" source=site.data.other-skills %}
</div>
