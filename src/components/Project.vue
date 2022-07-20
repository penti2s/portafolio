<template>
    <div id="container" class="mt-10 indigo lighten-1"> 
        <v-row justify="center"  >
            <v-col cols="12" xs="12" sm="12" md="12"> 
                <h1 class="text-center mt-15 text-h3 font-weight-medium"> Proyectos </h1> 
            </v-col>
            <v-col cols="12" sm="12" md="6" lg="4" >
                <CardProjects :data="project[0]" /> 
            </v-col>
            <v-col  cols="12" sm="12" md="6" lg="4">
                <CardProjects  :data="project[1]"/> 
            </v-col>
            <v-col  cols="12" sm="12" md="6" lg="4">
                <CardProjects :data="project[2]" />  
            </v-col>
        </v-row>
    </div>
</template>

<script>
import CardProjects from '@/components/CardProjects.vue'
export default {
    name: 'project-dev',
    data() {
        return {
            project: [
                {
                    name: 'Alfa-Web',
                    img: require('@/assets/proyecto1/img1.jpg'),
                    carrouseImg: [require('@/assets/proyecto1/img1.jpg'),require('@/assets/proyecto1/img2.jpg'),require('@/assets/proyecto1/img4.jpg'),require('@/assets/proyecto1/img5.jpg')],
                    description: 'Alfa-web es un desarrollo hecho dentro del bootcamp de talento digital, esta proyecto usa Vue.js y vuex para el manejo de datos y se desarrollo en el Framework de Vuetify de Vuejs.',
                    linkRepo: 'https://github.com/penti2s/alfa-web-dl',
                },
                {
                    name: 'Viajes Chile',
                    img: require('@/assets/proyecto2/img1.jpg'),
                    carrouseImg: [require('@/assets/proyecto2/img1.jpg'),require('@/assets/proyecto2/img2.jpg'),require('@/assets/proyecto2/img3.jpg'),],
                    description: 'Viajes chile es un web creada con HTML/CSS y JavaScript con bootrap, simula una web de viajes con lugares y actividades para realizar. Ademas cuenta con un formulario de contacto',
                    linkRepo: 'https://github.com/penti2s/viajes-chile',
                },
                {
                    name: 'Torneo de artes marciales',
                    img: require('@/assets/proyecto3/img1.jpg'),
                    carrouseImg: [require('@/assets/proyecto3/img1.jpg'),require('@/assets/proyecto3/img2.jpg'),require('@/assets/proyecto3/img3.jpg'),],
                    description: 'Web desarrollado con HTML/CSS y javascript pero esta vez usando programacion orientada a Objetos con su distribucion de herencias y metodos para el desarrollo de esta web de comparacion de poder de pelea de los luchadores de dragon ball Z',
                    linkRepo: 'https://github.com/penti2s/Torneo-Artes-Marciales',
                }
            ]
        }
    },
    components: {
        CardProjects,
    }
}
</script>

<style scoped>
    *{
        box-sizing: border-box;
        
    }
</style>