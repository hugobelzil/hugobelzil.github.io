---
title: Notes
subtitle: Short posts, technical notes, and announcements.
permalink: /posts/
---

{% if site.posts.size > 0 %}
  {% for post in site.posts %}
    <article class="post-list-item">
      <time class="post-date" datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%Y" }}</time>
      <div>
        <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
        {% if post.description %}
          <p>{{ post.description }}</p>
        {% endif %}
      </div>
    </article>
  {% endfor %}
{% else %}
  <p>No posts yet.</p>
{% endif %}
