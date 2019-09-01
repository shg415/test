<template>
    <p class="subtitle" v-html="subtitle"></p>
</template>

<script>
  export default{
    name: "ButtonSubtitle",
    props: {
      subtitle: {
        type: String,
        default: "noname"
      }
    }
  }
</script>

<style scoped lang="scss">
  .subtitle {
    font-size: 0.7rem;
    font-family: "FuturaPT";
    color: white;
    text-align: center;
    font-weight: bold;
  }


</style>
