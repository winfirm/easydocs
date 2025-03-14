# Easy Docs

## List
{% for post in site.posts limit:100 %} 
{% unless post.next %} 
  [{{ post.date | date: '%Y' }} {{ post.title }}](#!{{ post.title }}.md)  
{% endunless %} 
{% endfor %} 

## Help

help call
