<template>
  <div class="product-list">
    <h2 class="highlight-title">Một Số Sản Phẩm Nổi Bật</h2>
    <div class="product-grid">
      <div
        v-for="(product, index) in products"
        :key="index"
        class="product-item">
        <img
          :src="product.image"
          :alt="product.name"
          width="500"
          height="500" />
        <h3>{{ product.name }}</h3>
        <p class="product-description">{{ product.description }}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      products: [
        {
          name: "Espresso",
          image: "/img/espresso.png",
          description: "Cà phê đậm đặc đến từ Ý.",
        },
        {
          name: "Americano",
          image: "/img/americano.png",
          description: "Cà phê loãng phong cách Mỹ.",
        },
        {
          name: "Cappuccino",
          image: "/img/cappucino.png",
          description: "Sự kết hợp hoàn hảo giữa cà phê và sữa.",
        },
        {
          name: "Latte",
          image: "/img/latte.png",
          description: "Cà phê sữa mềm mại và thơm ngon.",
        },
        {
          name: "Mocha",
          image: "/img/mocha.png",
          description: "Hương vị chocolate đặc trưng.",
        },
        {
          name: "Macchiato",
          image: "/img/macchiato.png",
          description: "Cà phê pha chế kiểu Thổ Nhĩ Kỳ.",
        },
      ],
    };
  },
};
</script>

<style scoped>
.product-list {
  padding: 20px;
  text-align: center;
}

.highlight-title {
  color: brown;
  font-size: 24px;
  margin-bottom: 15px;
}

.product-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 20px;
}

.product-item {
  border: 1px solid #ddd;
  padding: 15px;
  text-align: center;
  background: #fff;
  border-radius: 5px;
}

.product-item img {
  max-width: 100%;
  height: auto;
  object-fit: contain;
}

.product-description {
  color: #666;
  margin: 10px 0;
}

@media (max-width: 768px) {
  .product-grid {
    grid-template-columns: repeat(2, 1fr);
  }
}

@media (max-width: 480px) {
  .product-grid {
    grid-template-columns: 1fr;
  }
}
</style>
