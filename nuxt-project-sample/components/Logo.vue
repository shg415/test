<template>
  <div id="app">
    <ul>
      <li v-for="item in items">
        {{ item.message }}
      </li>
    </ul>

  </div>
</template>



<script>
  export default{
    name:"items",
    data() {
      return{
        items: [
        { message: 'りんご' },
        { message: 'いちご' }
        ]
      };
    }
  };
</script>
