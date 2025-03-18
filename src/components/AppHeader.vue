<template>
  <div class="header">
    <div class="logo">
      <img src="/img/logo.png" alt="Coffee Logo" width="180" height="60" />
    </div>
    <nav>
      <ul>
        <li><a href="#">Trang Chủ</a></li>
        <li><a href="#">Giới Thiệu</a></li>
        <li><a href="#">Sứ Mệnh</a></li>
        <li><a href="#">Sản Phẩm</a></li>
      </ul>
    </nav>
  </div>
</template>

<style scoped>
body,
html {
  margin: 0;
  padding: 0;
}
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #4b2e2e;
  padding: 10px 20px;
  color: white;
  margin-bottom: 10px;
}
.logo img {
  width: 180px;
  height: 60px;
  object-fit: contain;
}
ul {
  list-style: none;
  display: flex;
  margin: 0;
  padding: 0;
}
li {
  margin-right: 15px;
}
a {
  text-decoration: none;
  color: white;
}
</style>
