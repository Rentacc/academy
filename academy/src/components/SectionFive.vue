<script></script>

<template>
    <div class="container">
  <div class="image-container">
    <img src="public/img/gallery-1-3(1).jpg" alt="">
    <div class="image-overlay">
      <div class="overlay-text">Driving Innovation</div>
    </div>
  </div>
  <div class="image-container">
    <img src="public/img/gallery-2-3(1).jpg" alt="">
    <div class="image-overlay">
      <div class="overlay-text">Driving Innovation</div>
    </div>
  </div>
  <div class="image-container">
    <img src="public/img/gallery-3-3(1).jpg" alt="">
    <div class="image-overlay">
      <div class="overlay-text">Driving Innovation</div>
    </div>
  </div>
  <div class="image-container">
    <img src="public/img/news-3-2.jpg" alt="">
    <div class="image-overlay">
      <div class="overlay-text">Driving Innovation</div>
    </div>
  </div>
</div>
</template>


<style scoped>
img{
    width: 375px;
    height: 255.91px;
}

.container {
  display: flex;
  flex-wrap: wrap;
}

.image-container {
  position: relative;
  
}

.image-container img {
    width: 375px;
    height: 255.91px;
}

.image-overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(255, 0, 0, 0.5); /* Sfondo semitrasparente rosso */
  display: flex;
  align-items: center;
  justify-content: center;
  opacity: 0;
  transition: opacity 0.3s ease;
}

.image-container:hover .image-overlay {
  opacity: 1;
}

.overlay-text {
  color: white;
  font-size: 18px;
  text-align: center;
}
</style>