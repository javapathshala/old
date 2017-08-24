---
layout: archive
permalink: /
author_profile: true
header:
  overlay_color: "#000"
  overlay_image: /assets/images/splash.jpg
  #overlay_filter: rgba(218,97,35,1)
  caption: Wisdom Being Shared
excerpt: '{::nomarkdown}<a href="https://www.facebook.com/sharer/sharer.php?u=https%3A//www.facebook.com/pathshalajava" class="btn btn--facebook"><i class="fa fa-fw fa-facebook" aria-hidden="true"></i><span> Facebook</span></a>
<a href="https://twitter.com/intent/tweet?via=javapathshala&text=www.javapathshala.com" class="btn btn--twitter" ><i class="fa fa-fw fa-twitter" aria-hidden="true"></i><span> Twitter</span></a>
<a href="https://plus.google.com/share?urls=aa" class="btn btn--google-plus"><i class="fa fa-fw fa-google-plus" aria-hidden="true"></i><span> Google+</span></a><a href="https://www.linkedin.com/shareArticle?mini=true&url=aa" class="btn btn--linkedin"><i class="fa fa-fw fa-linkedin" aria-hidden="true"></i><span> LinkedIn</span></a>
{:/nomarkdown}'
feature_row:
  - image_path: /assets/images/question.png
    #alt: "customizable"
    title: "Wisdom"
    excerpt: "Everything techical blog."
    url: "/posts/"
    btn_label: "Learn More"
  - image_path: /assets/images/mm-responsive-feature.png
    alt: "fully responsive"
    title: "Responsive Layouts"
    excerpt: "Built on HTML5 + CSS3. All layouts are fully responsive with helpers to augment your content."
    url: "/docs/layouts/"
    btn_label: "Learn More"
  - image_path: /assets/images/mm-free-feature.png
    alt: "100% free"
    title: "100% Free"
    excerpt: "Free to use however you want under the MIT License. Clone it, fork it, customize it, whatever!"
    url: "/docs/license/"
    btn_label: "Learn More"
github:
  - excerpt: '{::nomarkdown}<iframe style="display: inline-block;" src="https://ghbtns.com/github-btn.html?user=mmistakes&repo=minimal-mistakes&type=star&count=true&size=large" frameborder="0" scrolling="0" width="160px" height="30px"></iframe> <iframe style="display: inline-block;" src="https://ghbtns.com/github-btn.html?user=mmistakes&repo=minimal-mistakes&type=fork&count=true&size=large" frameborder="0" scrolling="0" width="158px" height="30px"></iframe>{:/nomarkdown}'
intro:
  - excerpt: ''
---
{% include subscribesidebar.html %}

{% include feature_row id="intro" type="center" %}

{% include feature_row %}

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
