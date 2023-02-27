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
  <ul>
  <li><h2>{{ post.title }}</h2>
  
  Published in <i>{{ post.venue }}</i> on {{ post.date | date: "%-d %B %Y" }} <br>
  <b>Abstract</b> {{post.excerpt}}<br>
    
  <b>Preferred Citation: </b>{{post.citation}}<br>
 </li>
 </ul>

  [Springer LCNS](https://link.springer.com/chapter/10.1007/978-3-031-04881-4_46){:.btn--research}
  [Arxiv Preprint](https://arxiv.org/pdf/2102.10555.pdf){:.btn--research}
  [Code](https://github.com/Farabi-shafkat/Improving-Action-Quality-Assessment-using-ResNets-and-Weighted-Aggregation){:.btn--research} <br>

{% endfor %}
