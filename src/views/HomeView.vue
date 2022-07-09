<template>
  <v-main>
    <Header />
    <AboutMe />
    <Project />
  </v-main>
</template>

<script>
  import Header from '@/components/Header.vue'
  import AboutMe from '@/components/AboutMe.vue'
  import Project from '@/components/Project.vue'
  export default {
    name: 'Home-view',

    components: {
      Header,
      AboutMe,
      Project,
    },
  }
</script>
