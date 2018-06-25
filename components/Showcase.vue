<template>
  <section id="showcase">
    <div class="container">
      <div class="row">
        <Projects heading="Side Hustle"/>
        <writing heading="Writing"/>
      </div>
    </div>
  </section>
</template>

<script>
import Projects from '@/components/Projects'
import Writing from '@/components/Writing'
export default {
  components: {
    Projects,
    Writing
  }
}
</script>

<style>
#showcase {
  background-color:#f6f9fc;
}

#showcase h1,
#showcase a {
  color: #24b47e;
}

#showcase h6 {
  font-family: 'Roboto Mono', monospace;
  font-size: 12px;
  margin-bottom: 25px;
}
.project,
.article {
   margin-bottom: 30px;
}

</style>


