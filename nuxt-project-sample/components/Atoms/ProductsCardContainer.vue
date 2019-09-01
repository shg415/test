<template>
  <div class="card">
    <slot></slot>
  </div>
</template>

<script>

</script>


<style scoped lang="scss">
.card {
  width: $wrap / 4 - 15 ;
  height: 198 * ($wrap / 4 - 15) / 323 * 2 ; //画像サイズ：323 * 198
  background-color: rgb(239, 239, 239);
}
</style>
