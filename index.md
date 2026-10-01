---
layout: default
---

{% include hero.html %}

<h2>Featured Projects</h2>

<div class="grid">
{% for project in site.projects %}
{% include card.html project=project %}
{% endfor %}
</div>

<h2>Currently</h2>

<article>
<ul>
<li>Building: Geometric Algebra Physics Engine</li>
<li>Creating: Danetian Academy</li>
<li>Writing: The Song of Danu</li>
</ul>
</article>

<h2>Latest Essays</h2>

{% for post in site.posts limit:3 %}
<article>
<h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
<p>{{ post.excerpt }}</p>
</article>
{% endfor %}
