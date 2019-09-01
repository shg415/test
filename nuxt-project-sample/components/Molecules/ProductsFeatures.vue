<template>
  <div>
    <ul>
      <li v-for="item in features" :key="item.title">
        <nuxt-link :to="item.path">
          <products-feature :title="item.title" />
        </nuxt-link>
      </li>
    </ul>
  </div>
</template>

<script>
import ProductsFeature from '~/components/Atoms/ProductsFeature.vue'
export default {
  components: {
    ProductsFeature
  },
  props: {
    features: {
      type: Array
    }
  }
}
</script>

<style scoped lang="scss">
ul {
  list-style: none;
  display: flex;
  padding: 0 0 30px;
  justify-content: center;
  align-items: center;

  >li {
    padding: 0 10px;

    a {
      text-decoration: none;
    }
  }
}
</style>
