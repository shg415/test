<template>
  <ul>
    <li v-for="item in resdev"  :key="item.title">
      <button-background :image="item.image" :title="item.title">
        <nuxt-link :to="item.path">
          <button-square class="square">
            <button-title :title="item.title"/>
            <button-subtitle :subtitle="item.subtitle" />
          </button-square>
        </nuxt-link>
      </button-background>
    </li>
  </ul>
</template>

<script>
import ButtonBackground from '~/components/Atoms/ButtonBackground.vue'
import ButtonSquare from '~/components/Atoms/ButtonSquare.vue'
import ButtonSubtitle from '~/components/Atoms/ButtonSubtitle.vue'
import ButtonTitle from '~/components/Atoms/ButtonTitle.vue'
export default {
  components: {
    ButtonBackground,
    ButtonSquare,
    ButtonSubtitle,
    ButtonTitle
  },
  props: {
    resdev: {
      type: Array,
    }
  }
}

</script>

<style scoped lang="scss">
ul{
  list-style: none;
  display: grid;
  grid-template-columns: $wrap/2-10 $wrap/2-10;
  grid-gap: 20px;
  width: $wrap;
  margin: 0 auto;
  padding: 0 0 45px 0;
}
</style>
