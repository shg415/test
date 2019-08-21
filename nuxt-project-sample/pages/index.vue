<template>
  <div class="container">
    <div>
      <div id="app">
      <button-vue>aaa</button-vue>
      </div>
      <heading-h1 />
      <logo />
      <h1 class="title">
        nuxt-project-sample
      </h1>
      <h2 class="subtitle">
        My remarkable Nuxt.js project
      </h2>
      <div class="links">
        <a
        href="https://nuxtjs.org/"
        target="_blank"
        class="button--green"
        >
        Documentation
      </a>
      <a
      href="https://github.com/nuxt/nuxt.js"
      target="_blank"
      class="button--grey"
      >
      GitHub
    </a>
  </div>
</div>
</div>
</template>

<script>
  import Logo from '~/components/Logo.vue'
  import HeadingH1 from '~/components/HeadingH1.vue'

  export default {
    components: {
      Logo,
      HeadingH1
    }
  }
</script>

<script>

  Vue.component("button-vue", {
    template: `
    <div class="button-vue">
      <slot></slot>
    </div>
    `
  });
  var app = new Vue({
    el: "#app"
  });
</script>



<style scoped lang="scss">
  .container {
    $background: #F5F5F5;
    margin: 0 auto;
    min-height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    background-color:$background;
  }

  .title {
    font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
    display: block;
    font-weight: 300;
    font-size: 100px;
    color: #35495e;
    letter-spacing: 1px;
  }

  .subtitle {
    font-weight: 300;
    font-size: 42px;
    color: #526488;
    word-spacing: 5px;
    padding-bottom: 15px;
  }

  .links {
    padding-top: 15px;
  }
</style>
