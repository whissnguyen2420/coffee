<template>
  <div>
    <AppHeader />
    <HomeHeroBanner />
    <AboutUs />
    <OurMission />
    <ProductList />
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import HomeHeroBanner from "./components/HomeHeroBanner.vue";
import AboutUs from "./components/AboutUs.vue";
import OurMission from "./components/OurMission.vue";
import ProductList from "./components/ProductList.vue";

export default {
  components: { AppHeader, HomeHeroBanner, AboutUs, OurMission, ProductList },
};
</script>
