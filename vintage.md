---
layout: default
title: Vintage Finds
permalink: /vintage/
---

# Vintage Finds

Welcome to my collection of quirky, character-filled vintage decor.  
Here you'll find stories, styling tips, and shopable treasures.  

---

## Stories & Finds

<div class="post-grid">
  {% for post in site.categories.vintage limit:6 %}
    <div class="post-card">
      <a href="{{ post.url }}">
        <div class="img-wrapper">
          <img src="{{ post.featured_image | default: '/assets/images/fallback.jpg' }}" alt="{{ post.title }}">
        </div>
        <h3>{{ post.title }}</h3>
      </a>
      <p class="post-date">{{ post.date | date: "%B %d, %Y" }}</p>
    </div>
  {% endfor %}
</div>

---

## Etsy Shop

<div class="listing-grid">
  <div class="listing">
    <a href="https://www.etsy.com/listing/4310565407/vintage-frog-candle-holder-bronze-finish" target="_blank">
      <img src="/assets/images/frogcandle.jpg" alt="Vintage Frog Candle Holder">
      <h3>Vintage Frog Candle Holder</h3>
      <p>$26 – Quirky bronze-finish frog on lily pad. Whimsical and functional.</p>
    </a>
  </div>

  <div class="listing">
    <a href="https://www.etsy.com/listing/4310330443/mid-century-pigeon-forge-pottery-owl" target="_blank">
      <img src="/assets/images/pigeonowl.jpg" alt="Pigeon Forge Pottery Owl">
      <h3>Pigeon Forge Pottery Owl</h3>
      <p>$48 – Mid-century handmade owl figurine. Studio pottery charm.</p>
    </a>
  </div>

  <div class="listing">
    <a href="https://www.etsy.com/listing/4297860317/vintage-hand-carved-wood-trivet-6-rustic" target="_blank">
      <img src="/assets/images/woodtrivet.jpg" alt="Wood Trivet">
      <h3>Wood Carved Trivet</h3>
      <p>$18 – 6” rustic hand-carved floral trivet. Functional and folk-style.</p>
    </a>
  </div>

  <div class="listing">
    <a href="https://www.etsy.com/listing/1884296024/vintage-solid-brass-duck-figurine-45" target="_blank">
      <img src="/assets/images/brassgoose.jpg" alt="Brass Duck Figurine">
      <h3>Brass Duck Figurine</h3>
      <p>$22 – 4.5” solid brass duck. Shiny and shelf-ready.</p>
    </a>
  </div>

  <div class="listing">
    <a href="https://www.etsy.com/listing/1892538115/blue-ceramic-bud-vase-bitossi-style" target="_blank">
      <img src="/assets/images/bluevase.jpg" alt="Blue Ceramic Bud Vase">
      <h3>Blue Ceramic Bud Vase</h3>
      <p>$32 – Bitossi-style texture and glaze. Eye-catching pop of color.</p>
    </a>
  </div>

  <div class="listing">
    <a href="https://www.etsy.com/listing/1878582944/vintage-brass-candlestick-holders-o-75" target="_blank">
      <img src="/assets/images/brasscandle.jpg" alt="Brass Candlestick Holders">
      <h3>Brass Candlestick Holders</h3>
      <p>$24 – Pair of heavy, low-profile holders. 0.75" taper.</p>
    </a>
  </div>
</div>
