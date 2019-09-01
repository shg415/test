<template>
  <div class="background">
    <slot></slot>
  </div>

</template>


<style scoped lang="css">
.background {
  width: 100%;
  background: url('~assets/img/ResDevBackground.png');
  background-size: cover;
}
</style>
