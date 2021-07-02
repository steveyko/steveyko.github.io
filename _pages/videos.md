---
layout: page
title: videos
permalink: /videos/
description: Videos for some of my projects
nav: false
---
<div class="videos">
    {% assign sorted_videos = site.videos | reverse %}
    <!-- Generate cards for each video -->
    <div class="container">
      <div class="row row-cols-1 row-cols-sm-2 row-cols-md-3 row-cols-lg-4">
        {% for video in sorted_videos %}
          {% include videos.html %}
        {% endfor %}
      </div>
    </div>
</div>
