<template>
  <section id="tech">
    <div class="container">
      <div class="row">
        <div class="col-md-12">
          <h1>{{title}}</h1>
        </div>
        <div v-for="item in tech" :key="tech[item]" class="col-md-4">
          <h3>[ {{ item.name }} ]</h3>
          <ul>
            <li v-for="skill in item.skills"  :key="skill"><i class="fas fa-check-circle"></i>{{ skill }}</li>
          </ul>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import tech from '@/data/tech'
export default {
  props:['title'],
  data () {
    return {
      tech
    }
  }
}
</script>

<style scoped>
h1 {
  text-align: center;
  margin-bottom: 50px;
  color: #6772e5;
}
li {
  list-style-type: none;
}
i {
  padding-right: 10px;
}
</style>
