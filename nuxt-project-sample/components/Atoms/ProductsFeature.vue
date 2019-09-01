<template>

  <div>
    <p>{{ title }}</p>
  </div>

</template>

<script>
export default {
  name: "ProductsFeature",
  props: {
    title: {
      type: String,
      default: "feature"
    }
  }
}

</script>

<style scoped lang="scss">

div {
  border-bottom: solid 3px rgb(239, 239, 239);
  width: 7.4vw;

  >p{
    font-size: 2rem;
    font-family: "YuGothic";
    color: rgb(0, 78, 162);
    font-weight: bold;
    text-align: center;
    padding: 4px 0;
  }
}
</style>
