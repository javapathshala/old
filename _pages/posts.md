---
layout: archive
permalink: /posts/
---
<div class="grid__wrapper">
<!-- {% capture written_year %}'None'{% endcapture %} -->
{% for post in site.posts %}
  <!-- {% capture year %}{{ post.date | date: '%Y' }}{% endcapture %} -->
  <!-- {% if year != written_year %}
    <h2 id="{{ year | slugify }}" class="archive__subtitle">{{ year }}</h2>
    {% capture written_year %}{{ year }}{% endcapture %}
  {% endif %} -->
  {% include archive-single.html type="grid" %}
{% endfor %}
</div>
<!-- <h3 class="archive__subtitle">{{ site.data.ui-text[site.locale].recent_posts | default: "Recent Posts" }}</h3>

<div class="grid__wrapper">
  {% for post in paginator.posts %}
  {% include archive-single.html type="grid" %}
{% endfor %}
</div>

{% include paginator.html %} -->
