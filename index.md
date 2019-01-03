---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---

{% for post in site.posts %}
<h2><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h2>
<p class="meta">{{ post.date|date_to_string }} | {{ post.author.first_name }} {{ post.author.last_name }}</p>
<div class="excerpt">{{ post.excerpt|safe }}</div>
<p class="meta"><a href="{{ site.basesurl }}{{ post.url }}">Read more &rarr;</a></p>
{% endfor %}
