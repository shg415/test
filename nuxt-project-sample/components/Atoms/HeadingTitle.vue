<template>
  <div>
    <h2 v-bind:class="headingstyle">{{ title }}</h2>
  </div>
</template>

<script>
  export default {
    name: "HeadingTitle",
    props: {
      title: {
        type: String,
        default: "noname"
      },
      headingstyle: {
        type: String,
        default: "blue"
      }
    }
  }
</script>

<style scoped lang="scss">
  h2{
    font-size: 3rem;
    font-family: "FuturaPT";

  }
  .blue {
    color: rgb(0, 78, 162);
  }
  .white {
    color: white;
  }
  .red{
    color:red;
  }
</style>
