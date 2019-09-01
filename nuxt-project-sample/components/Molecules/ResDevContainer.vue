<template>
  <div>
    <res-dev-background>
      <div class="heading">
        <heading-title title="RESERCH" headingstyle="blue" />
        <heading-title title="&" headingstyle="red" class="and" />
        <heading-title title="DEVELOPMENT" headingstyle="blue" />
      </div>
      <slot></slot>
    </res-dev-background>
  </div>
</template>

<script>
import HeadingTitle from '~/components/Atoms/HeadingTitle.vue'
import HeadingSubtitle from '~/components/Atoms/HeadingSubtitle.vue'
import ResDevBackground from '~/components/Atoms/ResDevBackground.vue'

export default {
  components: {
    HeadingTitle,
    HeadingSubtitle,
    ResDevBackground
  }
}

</script>

<style scoped lang="scss">
.heading {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 45px 0;
  .and {
    padding: 0 5px;
  }
}
</style>
