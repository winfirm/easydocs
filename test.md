---
layout: null
---

{% for post in site.posts limit:100 %} 
	{% unless post.next %} 
		<a href="{{ post.url }}">{{ post.date | date:"%Y-%m-%d" }} {{ post.title }}</a>
	{% endunless %} 
{% endfor %} 
