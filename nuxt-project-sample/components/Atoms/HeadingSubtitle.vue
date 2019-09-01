<template>
  <div>
    <p v-bind:class="headingstyle">{{ subtitle }}</p>
  </div>
</template>

<script>
  export default {
    name: "HeadingSubtile",
    props: {
      subtitle: {
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
  p{
    font-family: "YuGothic";
  }
  .blue {
    font-size: 2.2rem;
    color: rgb(146, 146, 146);
    padding: 0 15px;
  }
  .white {
    font-size:2rem;
    color: white;
    padding: 0 20px;
  }
  .red{
    color:red;
  }
</style>
