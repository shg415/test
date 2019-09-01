<template>
  <div id="news">
    <ul>
      <li v-for="item in items">
        <nuxt-link class="item" :to="item.path">
            <div class="title">
              <list-icon /><h2>{{ item.title }}</h2>
            </div>
            <p>{{ item.from }}{{ item.date }}<span>{{ item.point }}points</span></p>

        </nuxt-link>
      </li>
    </ul>

  </div>
</template>



<script>
  import ListIcon from '~/components/ListIcon.vue'
  export default{
    components: {
      ListIcon
    },
    name:"items",
    data() {
      return{
        items: [
        { title: "りんご", path: "/about", from:"TechCrunch Japan", date: "2019.08.20", point: 3},
        { title: "りんご", path: "/", from:"TechCrunch Japan", date: "2019.08.20", point: 3},
        { title: "りんご", path: "/", from:"TechCrunch Japan", date: "2019.08.20", point: 3},
        { title: "りんご", path: "/", from:"TechCrunch Japan", date: "2019.08.20", point: 3}
        ]
      };
    }
  };


</script>



<style scoped lang="scss">
  .item{
    text-decoration: none;
    color: black;
  }
  .title{
    display: flex;
    align-items: center;
  }

  ul{
    margin: 0 auto;
    padding: 0;
    > li{
      margin-bottom: 3px;
      background-color: white;
      list-style: none;
      padding: 10px 20px;

      h2{
        font-weight: normal;
        font-size: 14px;
        text-align: left;
        position: relative;
        line-height: 15px;
      }
      p{
        padding: 5px 28px;
        font-size: 8px;
        color: gray;
        text-align: left;
        line-height: 16px;

        span{
          color: $blue;
          font-size: 11px;
          background-color: $background;
          margin: 0 5px;
          padding: 1px 3px;
        }
      }
    }


  }


</style>
