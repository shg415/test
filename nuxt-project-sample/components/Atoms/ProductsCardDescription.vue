<template>
<div>
  {{ description }}
</div>


</template>

<script>
export default {
  name: "ProductsCardDescription",
  props: {
    description: {
      type: String,
      default: "description"
    }
  }
}


</script>


<style scoped lang="scss">
div {
    font-size: 1.6rem;
    font-family: "YuGothic";
    color: rgb(41, 41, 41);
    line-height: 1.8rem;
    text-align: center;
    height: 3.6rem;
}
</style>
