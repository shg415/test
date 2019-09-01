<template>
  <div>
    <products-container>
      <products-features :features="features" class="features" />
      <products-card :products="products" />
    </products-container>
  </div>
</template>

<script>
import ProductsCard from '~/components/Molecules/ProductsCard.vue'
import ProductsFeatures from '~/components/Molecules/ProductsFeatures.vue'
import ProductsContainer from '~/components/Molecules/ProductsContainer.vue'
export default {
  components: {
    ProductsCard,
    ProductsFeatures,
    ProductsContainer
  },
  data() {
    return{
      features: [
        { title: "断熱", path: "/about" },
        { title: "緩衝", path: "/about" },
        { title: "音", path: "/about" },
        { title: "成形", path: "/about" },
        { title: "耐熱", path: "/about" },
        { title: "シール性", path: "/about" }
      ],
      products: [
        { title: "ライトロン", image: require("~/assets/img/products-image.png"),
        description: "薄肉ながら基本特性に優れ、<br>ITモバイル機器などのスリム化に貢献", path: "/about" },
        { title: "ライトロン", image: require("~/assets/img/products-image.png"),
        description: "薄肉ながら基本特性に優れ、<br>ITモバイル機器などのスリム化に貢献", path: "/about" },
        { title: "ライトロン", image: require("~/assets/img/products-image.png"),
        description: "薄肉ながら基本特性に優れ、<br>ITモバイル機器などのスリム化に貢献", path: "/about" },
        { title: "ライトロン", image: require("~/assets/img/products-image.png"),
        description: "薄肉ながら基本特性に優れ、<br>ITモバイル機器などのスリム化に貢献", path: "/about" },
        { title: "ライトロン", image: require("~/assets/img/products-image.png"),
        description: "薄肉ながら基本特性に優れ、<br>ITモバイル機器などのスリム化に貢献", path: "/about" },
        { title: "ライトロン", image: require("~/assets/img/products-image.png"),
        description: "薄肉ながら基本特性に優れ、<br>ITモバイル機器などのスリム化に貢献", path: "/about" }
      ]
    };
  }
}
</script>

<style scoped lang="scss">
.features {
  margin: 0 auto;
}
</style>
