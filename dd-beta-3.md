---
layout: page
title: DD Beta 3
permalink: /dd-beta-3/
---

{% assign sorted_categories = site.categories | sort %}
{% for category in sorted_categories %}
   <h3 class="post-title"><a href="{{ site.baseurl }}/roinn-seorsa/{{ category | first }}" name="{{ category | first }}">{{ category | first }}</a></h3>
   <div class="section-divider"></div>
   <div class="row">
      {% for post in category.last limit:3 %}
         <div class="col-md-3">
            <p><a href="{{ site.baseurl }}{{ post.url }}"><img src="{{ post.image }}" class="index-image"></a></p>
            <h5 class="post-title"><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h5>
            <!-- If there is an autor link defined in the post's front matter link to that author -->
            {% if post.author %}
               <p class="text-muted">{{ post.date | date: "%Y-%m-%d" }} le <a href="{{ post.author_url }}">{{ post.author }}</a></p>
            <!-- If there is not auther defined in the post's front matter link to Crìstean MacMhìcheil -->
            {% else %}
               <p class="text-muted">{{ post.date | date: "%Y-%m-%d" }} le <a href="{{ site.baseurl}}/fios/">Crìstean MacMhìcheil</a></p>
            {% endif %}
            <!-- Insert the post excerpt here -->
            {{ post.excerpt }}
         </div>
         <div class="col-md-1"></div>
      {% endfor %}
         <div class="col-md-1">
            <p><a href="{{ site.baseurl }}/roinn-seorsa/{{ category | first }}" name="{{ category | first }}"><i class="fas fa-arrow-right"></i></a></p>
         </div>
   </div>
{% endfor %}
