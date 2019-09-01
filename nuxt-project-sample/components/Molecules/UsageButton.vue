<template>
  <ul>
    <li v-for="item in usage"  :key="item.title">
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
    usage: {
      type: Array,
    }
  }
}

</script>

<style scoped lang="scss">
ul{
  display: flex;
  list-style: none;
  margin: 0 4.5rem;
  padding: 0 0 60px 0;
  justify-content: space-between;
}
</style>
