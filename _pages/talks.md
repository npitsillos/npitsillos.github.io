---
layout: page
title: Talks
permalink: /talks/
nav: true
horizontal: false
---
<div class="talks">
  <!-- Display projects without categories -->
    {% assign sorted_talks = site.talks | sort: "importance" %}
    <!-- Generate cards for each project -->
    {% if page.horizontal %}
      <div class="container">
        <div class="row row-cols-2">
        {% for talk in sorted_talks %}
          {% include talks_hrz.html %}
        {% endfor %}
        </div>
      </div>
    {% else %}
      <div class="grid">
        {% for talk in sorted_talks %}
          {% include talks.html %}
        {% endfor %}
      </div>
    {% endif %}

</div>
