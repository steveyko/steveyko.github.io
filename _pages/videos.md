---
layout: page
title: videos
permalink: /videos/
description: Research-related videos
nav: true
---
<div class="videos">
    {% assign sorted_videos = site.videos | sort: "order" | reverse %}
    <!-- Generate cards for each video -->
    <div class="container">
      <div class="row row-cols-1 row-cols-sm-2">
        {% for video in sorted_videos %}
          {% include videos.html %}
        {% endfor %}
      </div>
    </div>
</div>
