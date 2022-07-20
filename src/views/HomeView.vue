<template>
  <v-main>
    <Header />
    <AboutMe />
    <Project />
    <Skills />
    <Footer />
    <div data-tf-popover="SwCtBezg" data-tf-button-color="#0445AF"
      data-tf-tooltip="Hey 👋&nbsp;&nbsp;Quieres contactarme? " data-tf-chat data-tf-medium="snippet" style="all:unset;">
    </div>
  </v-main>
</template>

<script>
import Header from '@/components/Header.vue'
import AboutMe from '@/components/AboutMe.vue'
import Project from '@/components/Project.vue'
import Skills from '@/components/Skills.vue'
import Footer from '@/components/Footer.vue'

export default {
  name: 'Home-view',

  components: {
    Header,
    AboutMe,
    Project,
    Skills,
    Footer
  },
  mounted(){
    let Script = document.createElement('script')
    Script.setAttribute('src', '//embed.typeform.com/next/embed.js')
    document.head.appendChild(Script)
  }
}
</script>
