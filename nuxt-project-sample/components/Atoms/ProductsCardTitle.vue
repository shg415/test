<template>
<div>
  <p>{{ title }}</p>
</div>


</template>

<script>
export default {
  name: "ProductsCardTitle",
  props: {
    title: {
      type: String,
      default: "title"
    }
  }
}


</script>


<style scoped lang="scss">
div {

  >p{
    font-size: 1.8rem;
    font-family: "YuGothic";
    color: rgb(0, 78, 162);
    font-weight: bold;
    text-align: center;
  }
}
</style>
