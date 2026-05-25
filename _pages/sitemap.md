---
layout: archive
title: "Sitemap"
permalink: /sitemap/
author_profile: true
---

{% include base_path %}

A list of all the pages found on the site. For robots, an [XML version]({{ base_path }}/sitemap.xml) is also available.

<h2>Main Pages</h2>
<ul>
  <li><a href="{{ base_path }}/">Home</a></li>
  <li><a href="{{ base_path }}/publications/">Publications</a></li>
  <li><a href="{{ base_path }}/talks/">Talks</a></li>
  <li><a href="{{ base_path }}/cv/">CV</a></li>
</ul>

<h2>Publications</h2>
{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}

<h2>Talks & Presentations</h2>
{% for post in site.talks reversed %}
  {% include archive-single.html %}
{% endfor %}
