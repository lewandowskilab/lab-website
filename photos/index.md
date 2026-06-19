---
title: Photos
---

# {% include icon.html icon="fa-solid fa-images" %}Photos

{%
  include photo-row.html
  photos=site.data.content.team.figures
  size=site.data.content.team.photos_size
  id="allphotos"
  mode="grid"
%}
