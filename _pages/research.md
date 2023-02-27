---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

<style type="text/css">
     #circle {
      width: 10px;
      height: 10px;
      -webkit-border-radius: 2.5px;
      -moz-border-radius: 2.5px;
      border-radius: 2.5px;
      background: black;
    }

    marg {
   
    margin: 20px;
   
    }
</style>

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}




{% for post in site.publications reversed %}
 {% include archive-single.html %}
  <ul>
  <li><h2>{{ post.title }}</h2>
  
  Published in <i>{{ post.venue }}</i> on {{ post.date | date: "%-d %B %Y" }} <br><br>
  <b>Abstract</b> {{post.excerpt}}<br><br>

  <b>Preferred Citation: </b>{{post.citation}}<br><br>
  <b>Website: </b>{{post.paperurl}}<br><br>
  <b>Download Link: </b>{{post.arxiv}}<br><br>

 </li>
 </ul>



{% endfor %}

