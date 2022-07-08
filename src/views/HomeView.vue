<template>
  <v-main>
    <Header />
    <AboutMe />
  
  </v-main>
</template>

<script>
  import Header from '@/components/Header.vue'
  import AboutMe from '@/components/AboutMe.vue'

  export default {
    name: 'Home-view',

    components: {
      Header,
      AboutMe,
    },
  }
</script>
