## Welcome to Hanni Studio!

<p style="font-size: 1.1rem; max-width: 700px; margin-bottom: 2rem;">
  <em>Curating quirky, character-filled vintage finds and fun DIY projects for a home that tells your story.</em>
</p>

## Recent Blog Posts

<div class="post-grid">
  {% for post in site.posts limit:3 %}
    <div class="post-card">
      <a href="{{ post.url }}">
        <div class="img-wrapper">
          <img 
            src="{{ post.featured_image | default: '/assets/images/fallback.jpg' }}" 
            onerror="this.onerror=null;this.src='/assets/images/fallback.jpg';" 
            alt="{{ post.title }}" 
            loading="lazy">
        </div>
        <h3>{{ post.title }}</h3>
        <p class="post-date">{{ post.date | date: "%B %d, %Y" }}</p>
      </a>
    </div>
  {% endfor %}
</div>
