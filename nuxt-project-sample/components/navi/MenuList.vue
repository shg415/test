<template>
  <div>
    <ul>
      <li v-for="menu in menulist">
        <menu-button v-bind:path="menu.path" v-bind:name="menu.name"/>
      </li>
    </ul>
  </div>
</template>


<script>
  import MenuButton from '~/components/navi/MenuButton.vue'
  export default {
    components: {
      MenuButton
    },
    name:"MenuList",
    data() {
      return{
        menulist: [
        { name: "りんご", path: "/about" },
        { name: "いちご", path: "/" },
        { name: "ぶどう", path: "/about" },
        { name: "なし", path: "/about" }
        ]
      };
    }
  };


</script>

<style scoped lang="scss">
  ul{
    list-style: none;
    display: flex;
    justify-content: space-between;
    >li{


    }
  }

</style>
