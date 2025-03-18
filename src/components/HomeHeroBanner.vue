<template>
  <div class="banner">
    <img src="/img/banner.png" alt="Coffee Banner" width="1920" height="1080" />
    <div class="overlay">
      <div class="slogan">
        <h1>Hương vị đậm đà - Trải nghiệm tinh tế</h1>
        <p>Thưởng thức cà phê ngon nhất từ khắp nơi trên thế giới</p>
      </div>
    </div>
  </div>
</template>

<style scoped>
.banner {
  position: relative;
  text-align: center;
  color: white;
  overflow: hidden;
  margin-bottom: 10px;
}

.banner img {
  width: 100%;
  height: auto;
  max-height: 70vh;
  object-fit: cover;
}

.overlay {
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  background-color: rgba(0, 0, 0, 0.6);
  width: 100%;
  height: 20%;
  display: flex;
  justify-content: center;
  align-items: center;
}

.slogan {
  text-align: center;
  max-width: 80%;
  text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.7);
}
</style>
