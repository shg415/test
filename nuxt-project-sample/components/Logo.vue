<template>
  <div id="news">
    <ul>
      <li v-for="item in items">
        <h2>{{ item.title }}</h2>
        <p>{{ item.from }}{{ item.date }}<span>{{ item.point }}points</span></p>
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
        { title: "りんご", from:"TechCrunch Japan", date: "2019.08.20", point: 3},
        { title: "りんご", from:"TechCrunch Japan", date: "2019.08.20", point: 3},
        { title: "りんご", from:"TechCrunch Japan", date: "2019.08.20", point: 3},
        { title: "りんご", from:"TechCrunch Japan", date: "2019.08.20", point: 3}
        ]
      };
    }
  };
</script>



<style scoped lang="scss">

    ul{
      margin: 0 auto;
      padding: 0;
    li{
      margin-bottom: 3px;
      background-color: white;
      list-style: none;
      padding: 10px 30px;


      h2{
        font-weight:normal;
        font-size: 14px;
        text-align: left;
        position:relative;
        &:before{
        content: "";
        position:absolute;
        left:-20px;
        top:2px;
        width:15px;
        height:15px;
        display: block;
        background: url('~assets/img/list-icon.png');
        background-size:contain;
        }
      }
      p{
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
