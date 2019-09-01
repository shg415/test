<template>
    <p class="title" v-html="title"></p>
</template>

<script>
  export default{
    name: "ButtonTitle",
    props: {
      title: {
        type: String,
        default: "noname"
      }
    }
  }
  </script>

  <style scoped lang="scss">
    .title {
      font-size: 1.8rem;
      font-family: "YuGothic";
      color: rgb(255, 255, 255);
      padding-bottom: 4px;
      text-align: center;
    }

  </style>
