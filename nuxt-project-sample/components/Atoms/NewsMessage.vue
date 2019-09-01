<template>
  <div>
    <p :class="category">{{ message }}</p>
  </div>
</template>

<script>
export default{
  name: "NewsMessage",
  props: {
    message: {
      type: String,
      default: "/"
    },
    category: {
      type: String,
      default: "/"
    }
  }
}

</script>

<style scoped lang="scss">
p{
  font-size: 1.4rem;
  text-align: left;
    font-family: "YuGothic";
}
.important {
  color: rgb(201, 14, 41);
}

.news {
  color: black;
}
.example {
  color: black;
}

</style>
