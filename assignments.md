---
layout: page
---
<!---
This iterates over the assignments collection. For more information about 
collections in Jekyll see https://jekyllrb.com/docs/collections/ 
--->
{% for assignment in site.assignments %}
 <h3>{{ assignment.name }}</h3>
 <p>
  {{ assignment.description | markdownify }}
  <a href="{{ assignment.link | relative_url }}">LINK</a>
 </p>
{% endfor %}
