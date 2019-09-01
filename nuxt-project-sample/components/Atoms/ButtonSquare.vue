<template>
  <div>
    <slot></slot>
  </div>
</template>

<style scoped lang="scss">
  div{
    background-color: rgb(0, 78, 162);
    width: 8.5vw;
    height: 8.5vw;
    display:flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translateY(-50%) translateX(-50%);
  }


</style>
