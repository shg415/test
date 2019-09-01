<template>
  <div>
    <app-background background="white">
      <div class="heading">
        <heading-title title="PRODUCTS" headingstyle="blue" />
        <heading-subtitle subtitle="セキスイの発泡体" headingstyle="blue" />
      </div>
      <slot></slot>
    </app-background>
  </div>
</template>

<script>
import AppBackground from '~/components/Atoms/AppBackground.vue'
import HeadingTitle from '~/components/Atoms/HeadingTitle.vue'
import HeadingSubtitle from '~/components/Atoms/HeadingSubtitle.vue'


export default {
  components: {
    AppBackground,
    HeadingTitle,
    HeadingSubtitle
  }
}

</script>

<style scoped lang="scss">
.heading {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 45px 0;

}
</style>
