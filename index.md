# Welcome to my website!

I'll be publishing weekly blog posts on topics that interest me, new technology I come across, current events, and more.

Stay tuned for my first post. 😎

# Blog

{% for post in site.posts %}
  <a href="{{ post.url }}" title="{{ post.title }}">
    <div class="posts">
      <h3>{{ post.title }}</h3>
      <span>{{ post.date | date_to_string }}</span>
    </div>
  </a>
{% endfor %}
