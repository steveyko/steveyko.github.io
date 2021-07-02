---
layout: page
title: videos
permalink: /videos/
description: Videos for some of my projects
nav: false
horizontal: false
---
<div class="projects">
    {% assign sorted_videos = site.videos | reverse %}
    <!-- Generate cards for each video -->
    {% if page.horizontal %}
      <div class="container">
        <div class="row row-cols-2">
        {% for video in sorted_videos %}
          {% include videos_hrz.html %}
        {% endfor %}
        </div>
      </div>
    {% else %}
      <div class="grid">
        {% for video in sorted_videos %}
          {% include videos.html %}
        {% endfor %}
      </div>
    {% endif %}
</div>
