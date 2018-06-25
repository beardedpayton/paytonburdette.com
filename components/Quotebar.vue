<template>
  <section id="quotebar">
    <div class="container">
      <div class="col-md-12">
        <p>{{quote}}</p>
      </div>
    </div>
  </section>
</template>

<script>
import quotes from '@/data/quotes'
export default {
  data() {
    return {
      quotes,
      quote: quotes[Math.floor(Math.random()*quotes.length)]
   }
  }
}
</script>

<style scoped>
#quotebar {
  font-size: 14px;
  background-color: #f6f9fc;
  padding: 0;
  text-align: center;
}

</style>
