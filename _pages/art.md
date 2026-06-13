---
title: Art
description: Francesca Greenstreet's paintings and artwork.
permalink: /art
---

<div class="art-grid">
  <div class="art-item"><img src="/images/art/painting-cesca.jpeg.webp" alt="Painting" loading="lazy"></div>
  <div class="art-item"><img src="/images/art/IMG_8863_converted.webp" alt="Painting" loading="lazy"></div>
  <div class="art-item"><img src="/images/art/bath-leg.webp" alt="Painting" loading="lazy"></div>
  <div class="art-item"><img src="/images/art/IMG_0340_converted.webp" alt="Painting" loading="lazy"></div>
  <div class="art-item"><img src="/images/art/IMG_9494_converted.webp" alt="Painting" loading="lazy"></div>
  <div class="art-item"><img src="/images/art/IMG_8999_converted.webp" alt="Painting" loading="lazy"></div>
  <div class="art-item"><img src="/images/art/IMG_2822_converted.webp" alt="Painting" loading="lazy"></div>
  <div class="art-item"><img src="/images/art/37089CB4-C25F-4270-BC73-DA01D4AF44DF.webp" alt="Painting" loading="lazy"></div>
  <div class="art-item"><img src="/images/art/IMG_8699_converted.webp" alt="Painting" loading="lazy"></div>
  <div class="art-item"><img src="/images/art/IMG_8145_converted.webp" alt="Painting" loading="lazy"></div>
  <div class="art-item"><img src="/images/art/IMG_8152_converted.webp" alt="Painting" loading="lazy"></div>
  <div class="art-item"><img src="/images/art/IMG_8423_converted.webp" alt="Painting" loading="lazy"></div>
  <div class="art-item"><img src="/images/art/IMG_1476_converted.webp" alt="Painting" loading="lazy"></div>
</div>

<div class="lightbox" id="lightbox">
  <span class="lightbox-close">&times;</span>
  <img class="lightbox-image" id="lightbox-image" src="" alt="Painting">
</div>

<style>
.art-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 8px;
  max-width: 900px;
  margin: 0 auto;
}

.art-item {
  aspect-ratio: 1;
  overflow: hidden;
  cursor: pointer;
  transition: transform 0.2s ease;
}

.art-item:hover {
  transform: scale(1.02);
}

.art-item img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

@media (max-width: 600px) {
  .art-grid {
    grid-template-columns: repeat(2, 1fr);
    gap: 4px;
  }
}

.lightbox {
  display: none;
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(0, 0, 0, 0.9);
  z-index: 1000;
  justify-content: center;
  align-items: center;
}

.lightbox.active {
  display: flex;
}

.lightbox-image {
  max-width: 90%;
  max-height: 90%;
  object-fit: contain;
}

.lightbox-close {
  position: absolute;
  top: 20px;
  right: 30px;
  font-size: 40px;
  color: white;
  cursor: pointer;
  z-index: 1001;
}

.lightbox-close:hover {
  color: #ccc;
}
</style>

<script>
document.addEventListener('DOMContentLoaded', function() {
  const lightbox = document.getElementById('lightbox');
  const lightboxImage = document.getElementById('lightbox-image');
  const artItems = document.querySelectorAll('.art-item img');

  artItems.forEach(function(img) {
    img.addEventListener('click', function() {
      lightboxImage.src = this.dataset.full || this.src;
      lightbox.classList.add('active');
    });
  });

  lightbox.addEventListener('click', function(e) {
    if (e.target === lightbox || e.target.classList.contains('lightbox-close')) {
      lightbox.classList.remove('active');
    }
  });

  document.addEventListener('keydown', function(e) {
    if (e.key === 'Escape') {
      lightbox.classList.remove('active');
    }
  });
});
</script>
