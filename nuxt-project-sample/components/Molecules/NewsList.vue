<template>
  <ul>
    <li v-for="item in news" :key="item.title">
      <news-container class="container">
        <news-date :date="item.date" />
        <news-category :category="item.category" class="category" />
        <news-message :message="item.message" :category="item.category" />
      </news-container>
    </li>
  </ul>

</template>
<script>
import NewsDate from '~/components/Atoms/NewsDate.vue'
import NewsCategory from '~/components/Atoms/NewsCategory.vue'
import NewsMessage from '~/components/Atoms/NewsMessage.vue'
import NewsContainer from '~/components/Atoms/NewsContainer.vue'
export default {
  components: {
    NewsDate,
    NewsCategory,
    NewsMessage,
    NewsContainer


  },
  name: "NewsList",
  props: {
    news: {
      type: Array
    }
  }
}
</script>

<style scoped lang="scss">
ul {
  list-style: none;
  width: $wrap;
  margin: 0 auto;
  padding: 0;
  .category {
    margin: 0 10px;
  }

}



</style>
<!--

import  from '~/components/Atoms/.vue'
-->
