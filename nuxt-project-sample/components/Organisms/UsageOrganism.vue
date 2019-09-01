<template>

  <usage-container>
        <usage-button :usage="usage" />
  </usage-container>
</template>

<script>
import UsageButton from '~/components/Molecules/UsageButton.vue'
import UsageContainer from '~/components/Molecules/UsageContainer.vue'
export default {
  components: {
    UsageButton,
    UsageContainer,

  },
  name: "usage",
  data() {
    return{
      usage: [
        { title: "建築土木", subtitle: "Building<br>&<br>Construction", image: require("~/assets/img/usage-background.png"), path: "/about",  },
        { title: "テープ", subtitle: "Tape", image: require("~/assets/img/usage-background.png"), path: "/about",  },
        { title: "輸送機器", subtitle: "Automotive<br>&<br>Industrial", image: require("~/assets/img/usage-background.png"), path: "/about",  },
        { title: "ITデバイス", subtitle: "IT", image: require("~/assets/img/usage-background.png"), path: "/about",  },
        { title: "その他", subtitle: "Other", image: require("~/assets/img/usage-background.png"), path: "/about",  },
      ]
    };
  }
}

</script>
<style scoped lang="scss">

</style>
