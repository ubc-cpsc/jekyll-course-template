---
layout: page
---
<!---
This iterates over the tutorials collection. For more information about 
collections in Jekyll see https://jekyllrb.com/docs/collections/ 
--->
{% for tutorial in site.tutorials %}
 <h3>{{ tutorial.name }}</h3>
 <p>
  {{ tutorial.description | markdownify }}
  <a href="{{ tutorial.url | relative_url }}">LINK</a>
 </p>
{% endfor %}
