<template>
  <div :class="background">
    <slot></slot>
  </div>

</template>

<script>
export default {
  name: "AppBackground",
  props: {
    background: {
      type: String,
      default: "white;"
    }
  }
}

</script>

<style scoped lang="scss">
.white {
  background-color: white;
}
.blue {
  background-color: rgb(9, 33, 108);
}
.gray {
  background-color: rgb(233, 236, 243);
}
</style>
