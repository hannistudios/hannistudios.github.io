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
      <img src="https://i.etsystatic.com/49013698/r/il/5ef3eb/5803374423/il_794xN.5803374423_9mdp.jpg" alt="Vintage Frog Candle Holder">
      <h3>Vintage Frog Candle Holder</h3>
      <p>$26 – Quirky bronze-finish frog on lily pad. Whimsical and functional.</p>
    </a>
  </div>

  <div class="listing">
    <a href="https://www.etsy.com/listing/4310330443/mid-century-pigeon-forge-pottery-owl" target="_blank">
      <img src="https://i.etsystatic.com/49013698/r/il/5c6c85/5803329289/il_794xN.5803329289_9bqg.jpg" alt="Pigeon Forge Pottery Owl">
      <h3>Pigeon Forge Pottery Owl</h3>
      <p>$48 – Mid-century handmade owl figurine. Studio pottery charm.</p>
    </a>
  </div>

  <div class="listing">
    <a href="https://www.etsy.com/listing/4297860317/vintage-hand-carved-wood-trivet-6-rustic" target="_blank">
      <img src="https://i.etsystatic.com/49013698/r/il/e9cbd7/5776171193/il_794xN.5776171193_9fop.jpg" alt="Wood Trivet">
      <h3>Wood Carved Trivet</h3>
      <p>$18 – 6” rustic hand-carved floral trivet. Functional and folk-style.</p>
    </a>
  </div>

  <div class="listing">
    <a href="https://www.etsy.com/listing/1884296024/vintage-solid-brass-duck-figurine-45" target="_blank">
      <img src="https://i.etsystatic.com/49013698/r/il/1845b2/5527830864/il_794xN.5527830864_o8ux.jpg" alt="Brass Duck Figurine">
      <h3>Brass Duck Figurine</h3>
      <p>$22 – 4.5” solid brass duck. Shiny and shelf-ready.</p>
    </a>
  </div>

  <div class="listing">
    <a href="https://www.etsy.com/listing/1892538115/blue-ceramic-bud-vase-bitossi-style" target="_blank">
      <img src="https://i.etsystatic.com/49013698/r/il/3a90c7/5597014872/il_794xN.5597014872_exu5.jpg" alt="Blue Ceramic Bud Vase">
      <h3>Blue Ceramic Bud Vase</h3>
      <p>$32 – Bitossi-style texture and glaze. Eye-catching pop of color.</p>
    </a>
  </div>

  <div class="listing">
    <a href="https://www.etsy.com/listing/1878582944/vintage-brass-candlestick-holders-o-75" target="_blank">
      <img src="https://i.etsystatic.com/49013698/r/il/e3e76e/5500500730/il_794xN.5500500730_b48q.jpg" alt="Brass Candlestick Holders">
      <h3>Brass Candlestick Holders</h3>
      <p>$24 – Pair of heavy, low-profile holders. 0.75" taper.</p>
    </a>
  </div>
</div>
