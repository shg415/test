<template>
  <div class="button-container">

    <div class="button">
      {{ title }}
    </div>

  </div>
</template>


<script>
  export default {
    props: {
      title: {
        type: String,
        default: "default button"
      }
    }
  }


</script>

<style scoped lang="scss">

  .button{
    color: $blue;
    font-size: 16px;
    background-color:$background;
    margin:5px;
    padding:5px;
    display:block;
    vertical-align:middle;
  }
  .button-container{
    background-color:white;
    display: inline-block;
    vertical-align:middle;
    width:100%;

  /*上下中央揃え*/
  }

</style>
