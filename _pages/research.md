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

{% endfor %}

