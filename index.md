---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---

Hi

<ul>
  {% for post in site.posts %}
    <li>
      {{post.date | date: "%d %b %y"}} - <a href="{{ post.url }}">{{ post.title }}</a> - {% for tag in post.tags %} #{{tag}}{% endfor %} 
    </li>
  {% endfor %}
</ul>
