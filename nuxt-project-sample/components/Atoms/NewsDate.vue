<template>
  <div>
    <p class="date">{{ date }}</p>
  </div>
</template>

<script>
export default　{
  name: "NewsDate",
  props: {
    date: {
      type: String,
      default: "/"
    }
  }
}
  </script>

  <style scoped lang="scss">
  .date {
    font-size: 1.4rem;
    font-family: "YuGothic";
  }

  </style>
