<template>
  <section id="bio">
    <div class="container">
      <div class="row">
        <div class="col-md-6">
          <h1>{{ info.intro }}</h1>
          <p v-for="paragraph in info.bio" :key="paragraph">{{ paragraph }}</p>
        </div>
         <div class="col-md-6 d-flex justify-content-end">
           <img src="../static/payton-circle.png" :alt="info.name">
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import info from '@/data/info'
export default {
 props:['info']
}
</script>

<style>
  @media (max-width: 767px) {
    img {
      margin: 0 auto;
      margin-top: 50px;
    }
  }
</style>
