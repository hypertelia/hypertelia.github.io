<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <img src="{{ site.baseurl }}/{{ post.image }}">
      <p>{{ post.excerpt | strip_html }} <a href="{{ post.url }}">Read more …</a></p>
    </li>
  {% endfor %}
</ul>