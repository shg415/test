<template>
  <div>
    <ul>
      <li v-for="item in products" :key="item.title">
        <products-card-container>
          <products-card-image :image="item.image" :title="item.title" />
          <products-card-title :title="item.title" class="title" />
          <products-card-description v-html:description="item.description" class="description" />
          <nuxt-link :to="item.path">
            <products-card-button class="button" />
          </nuxt-link>
        </products-card-container>
      </li>
    </ul>
  </div>
</template>

<script>
import ProductsCardButton from '~/components/Atoms/ProductsCardButton.vue'
import ProductsCardTitle from '~/components/Atoms/ProductsCardTitle.vue'
import ProductsCardDescription from '~/components/Atoms/ProductsCardDescription.vue'
import ProductsCardImage from '~/components/Atoms/ProductsCardImage.vue'
import ProductsCardContainer from '~/components/Atoms/ProductsCardContainer.vue'

export default {
  components: {
    ProductsCardButton,
    ProductsCardTitle,
    ProductsCardDescription,
    ProductsCardImage,
    ProductsCardContainer
  },
  props: {
    products: {
      type: Array
    }
  }
}

</script>

<style scoped lang="scss">
ul {
  list-style: none;
  display: grid;
  grid-template-columns: $wrap/4-15 $wrap/4-15 $wrap/4-15 $wrap/4-15;
  grid-gap: 20px;
  width: $wrap;
  margin: 0 auto;
  padding: 0 0 45px 0;

  >li{
    margin: 0 auto;

  }

  .title {
    margin-top: 15px;
  }
  .description {
    margin-top: 15px;
  }
  .button {
    margin: 15px auto;
  }
  a{
    text-decoration: none;
  }
}
</style>
