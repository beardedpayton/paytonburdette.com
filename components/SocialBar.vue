<template>
  <section id="social-bar">
    <div class="container">
      <div class="row">
        <div class="col-md-6">
          <h4>Connect With Me</h4>
        </div>
        <div class="col-md-6 d-flex justify-content-end">
          <li v-for="item in social" :key="social[item]">
            <a :href="item.url"><i :class="item.icon"></i></a>
          </li>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  props:['social']
}
</script>

<style scoped>
  #social-bar {
    padding: 15px 0;
    background-color: #6772e5;
  }
  li {
    display: inline;
    list-style-type: none;
    padding-right: 30px;
  }
  h4,
  i {
    color: #fff;
  }
  i:hover {
    color: #222548;
  }
</style>

