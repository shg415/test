<template>
  <div v-if="category == 'news'" :class="category" class="category">
    <p>お知らせ</p>
  </div>

  <div v-else-if="category == 'important'" :class="category" class="category">
    <p>重要なお知らせ</p>
  </div>

  <div v-else-if="category == 'example'" :class="category" class="category">
    <p>導入事例</p>
  </div>

</template>

<script>
export default {
    name: "NewsCategory",
    props: {
      category: {
        type: String,
        default: "default"
      }
    }
  }

</script>

<style scoped lang="scss">
.category{
  width: 110px;

  >p {
    font-size: 1rem;
    font-family: "YuGothic";
    text-align: center;
    padding: 2px;
  }
}

.important {
  background-color: rgb(201, 14, 41);
  >p {
    color: white;
  }
}
.example {
    background-color: white;
    border: 1px solid rgb(0, 78, 162);
  >p {
    color: rgb(0, 78, 162);
  }
}

.news {
  background-color: rgb(0, 78, 162);
  >p {
    color: white;

  }
}

</style>
