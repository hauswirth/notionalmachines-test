# Notional Machines Collection
This web site hosts the notional machines collected by the ITiCSE'20 Working Group.

[Variable as Box]({% post_url 2020-06-16-VariableAsBox %})


## All Notional Machines
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>


## Notional Machines by Tag
We organized the notional machines by tags.

{% for tag in site.tags %}
  <h3>{{ tag[0] }}</h3>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
