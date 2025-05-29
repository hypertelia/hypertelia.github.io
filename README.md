<ul>
  {% for post in site.posts %}
    <li>
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      {% if post.image %} 
      <img src="{{ post.image }}">
      {% endif %}
      <p>{{ post.excerpt | strip_html }} <a href="{{ post.url }}">Read more …</a></p>
    </li>
  {% endfor %}
</ul>