<template>
  <div>
    <res-dev-container>
      <res-dev-button :resdev="resdev" />
    </res-dev-container>
  </div>
</template>

<script>
import ResDevButton from '~/components/Molecules/ResDevButton.vue'
import ResDevContainer from '~/components/Molecules/ResDevContainer.vue'

export default {
  components: {
    ResDevButton,
    ResDevContainer
  },
  name: "resdev",
  data() {
    return{
      resdev: [
        { title: "ソフトロンの<br>技術", subtitle: "Softlon", image: require("~/assets/img/ResDev.png"), path: "/about",  },
        { title: "新たな技術への<br>取り組み", subtitle: "Reserch&<br>Development", image: require("~/assets/img/ResDev.png"), path: "/about",  },
      ]
    };
  }
}

</script>
<style scoped lang="scss">

</style>
