<template>
  <div class="col-md-6 projects">
    <h1>{{ heading }}</h1>
    <h6>I either wrote or contribute to</h6>
    <div v-for="project in projects" :key="projects[project]" class="project">
      <h4>{{ project.name }}</h4>
      <p>{{ project.brief }}</p>
      <p><i class="fas fa-link"></i><a :href="project.url">{{ project.url }}</a></p>
    </div>
  </div>
</template>

<script>
import projects from '@/data/projects'
export default {
  props: ['heading'],
  data () {
    return {
      projects
    }
  }
}
</script>

<style scoped>
.projects {
  border-right: 1px solid #e6e9ec;
}
i {
  padding-right: 10px;
}
</style>
