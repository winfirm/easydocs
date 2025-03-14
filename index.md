# Easy Docs

## List
{% for post in site.posts} 
[{{ post.date | date: '%Y' }} {{ post.title }}](#!{{ post.title }}.md)  
{% endfor %} 

## Help

help call
