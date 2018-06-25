<template>
  <div class="col-md-6">
    <h1>{{ heading }}</h1>
    <h6>I like to write sometimes</h6>
    <div v-for="article in writing" :key="writing[article]" class="article">
      <h4>{{ article.title }}</h4>
      <p><i class="fas fa-link"></i><a :href="article.url">Medium Article</a></p>
    </div>
  </div>
</template>

<script>
import writing from '@/data/writing'
export default {
  props: ['heading'],
  data () {
    return {
      writing
    }
  }
}
</script>

<style scoped>
a {
  padding-left: 10px;
}
</style>
