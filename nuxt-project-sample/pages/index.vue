<template>
  <div>

    <usage-organism />
    <products-organism />
    <resdev-organism />
    <news-organism />
  </div>
</template>

<script>
import UsageOrganism from '~/components/Organisms/UsageOrganism.vue'
import ProductsOrganism from '~/components/Organisms/ProductsOrganism.vue'
import ResdevOrganism from '~/components/Organisms/ResdevOrganism.vue'
import NewsOrganism from '~/components/Organisms/NewsOrganism.vue'

export default {
  components: {
    UsageOrganism,
    ProductsOrganism,
    ResdevOrganism,
    NewsOrganism
  }
}


</script>

<style scoped lang="scss">
</style>
