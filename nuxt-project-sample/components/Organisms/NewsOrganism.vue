<template>
  <div>
    <news-list :news="news" />
  </div>

</template>

<script>
import NewsList from '~/components/Molecules/NewsList.vue'

export default {
  components: {
    NewsList
  },
  data() {
    return{
      news: [
        { message: "新着ニュースです。", date: "2019.09.01", category: "news", },
        { message: "新着ニュースです。", date: "2019.09.01", category: "example", },
        { message: "新着ニュースです。", date: "2019.09.01", category: "important" },
      ]
    };
  }
}
</script>
