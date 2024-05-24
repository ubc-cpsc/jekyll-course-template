---
layout: page
---
<!---
This iterates over the lectures collection. For more information about 
collections in Jekyll see https://jekyllrb.com/docs/collections/ 
--->
{% for lecture in site.lectures %}
 <h3>{{ lecture.name }}</h3>
 <p>
  {{ lecture.description | markdownify }}
  <a href="{{ lecture.link | relative_url }}">SLIDES</a>
 </p>
{% endfor %}
