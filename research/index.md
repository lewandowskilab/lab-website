---
title: Research
nav:
  order: 1
  tooltip: Published works
---

# {% include icon.html icon="fa-solid fa-microscope" %}Research

{{ site.data.content.research.intro }}

{% include section.html %}

## {{ site.data.content.research.highlighted_heading }}

{% for paper in site.data.content.research.highlighted %}
{% include citation.html lookup=paper style="rich" %}
{% endfor %}

{% if site.data.content.research.videos.size > 0 %}

{% include section.html %}

## {{ site.data.content.research.videos_heading }}

{%
  include video-row.html
  videos=site.data.content.research.videos
  limit=site.data.content.research.videos_max
  width=site.data.content.research.videos_size
  id="research"
%}

{% if site.data.content.research.videos.size > site.data.content.research.videos_max %}
{%
  include button.html
  link="videos"
  text="More videos"
  icon="fa-solid fa-arrow-right"
  flip=true
%}
{% endif %}

{% endif %}

{% include section.html %}

## {{ site.data.content.research.all_heading }}

{% include search-box.html %}

{% include search-info.html %}

{% include list.html data="citations" component="citation" style="rich" %}
