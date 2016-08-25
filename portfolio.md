---
layout: page
title: portfolio
permalink: /portfolio/
---

{% for project in site.portfolio %}

{% if project.redirect %}
<div class="project">
    <div class="thumbnail">
        <a href="{{ project.redirect }}" target="_blank">
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}    
        <span>
            <h1>{{ project.title }}</h1>
            <br/>
            <p>{{ project.description }}</p>
        </span>
        </a>
    </div>
</div>
{% else %}

<div class="project ">
    <div class="thumbnail">
        <a href="{{ site.baseurl }}{{ project.url }}">
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}    
        <span>
            <h1>{{ project.title }}</h1>
            <br/>
            <p>{{ project.description }}</p>
        </span>
        </a>
    </div>
</div>

{% endif %}

{% endfor %}
<br/>
<hr/>
<br/>
<span class="contacticon center">
	<a href="http://duanemcpherson.com/contact/"><i class="fa fa-envelope-square"></i></a>
   	<a href="https://www.linkedin.com/in/duane-mcpherson" target="_blank"><i class="fa fa-linkedin-square"></i></a>
    <a href="http://vimeo.com/duanemcpherson" target="_blank"><i class="fa fa-vimeo-square"></i></a>
    <a href="http://dmcmodelling.tumblr.com/" target="_blank"><i class="fa fa-tumblr-square"></i></a>
	<a href="https://twitter.com/duanemcpherson" target="_blank"><i class="fa fa-twitter-square"></i></a>
</span>

<div class="col three caption">
	Please use one of the above links to get in contact with me :)
</div>