## Welcome to Hanni Studio!

## Recent Blog Posts

<div class="post-grid">
  {% for post in site.posts limit:3 %}
    <div class="post-card">
      <a href="{{ post.url }}">
        <img src="{{ post.featured_image | default: '/assets/images/fallback.jpg' }}" alt="{{ post.title }}" loading="lazy">
        <h3>{{ post.title }}</h3>
      </a>
      <p class="post-date">{{ post.date | date: "%B %d, %Y" }}</p>
    </div>
  {% endfor %}
</div>
