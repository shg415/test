<template>
  <div>
    <app-background background="blue">
      <div class="heading">
        <heading-title title="USAGE" headingstyle="white" />
        <heading-subtitle subtitle="用途でさがす" headingstyle="white" />
      </div>
      <slot></slot>
    </app-background>
  </div>
</template>

<script>
import HeadingTitle from '~/components/Atoms/HeadingTitle.vue'
import HeadingSubtitle from '~/components/Atoms/HeadingSubtitle.vue'
import AppBackground from '~/components/Atoms/AppBackground.vue'

export default {
  components: {
    HeadingTitle,
    HeadingSubtitle,
    AppBackground
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
