<template>
  <div>
    <img :src="image" :alt="title">
  </div>
</template>

<script>
export default {
  name: "ProductsCardImage",
  props: {
    title: {
      type: String,
      default: "title"
    },
    image: {
      type: String,
      default: "noimage"
    }
  }
}
</script>


<style scoped lang="scss">
img{
  max-width: 100%;
  height: auto;
}
</style>
