<template>
  <div>
    <nuxt-link class="menu-button" v-bind:to="path">{{ name }}</nuxt-link>
  </div>
</template>

<script>
  export default {
    props: {
      path: {
        type: String,
        default: "/"
      },
      name: {
        type: String,
        default: "noname"
      }
    }
  }

</script>



<style scoped lang="scss">
  .menu-button {
    font-size: 14px;
    font-family: "NotoSansCJKjp";
    text-decoration: none;
    color: black;
    font-weight: bold;
  }

</style>
