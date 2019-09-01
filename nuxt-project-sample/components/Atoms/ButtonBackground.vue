<template>
  <div>
    <img v-bind:src="image" v-bind:alt="title">
    <slot></slot>
  </div>
</template>

<script>
export default{
  name: "ButtonBackground",
  props: {
    image: {
      type: String,
      default: "/"
    },
    title: {
      type: String,
      default: "noname"
    }
  }
}


</script>

<style scoped lang="scss">
div{
  position: relative;

  img{
    max-width: 100%;
    height: auto;
  }
}

</style>
