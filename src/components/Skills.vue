<template>
    <div class="d-flex flex-column   justify-center ">  >
        <h1 class="text-center white--text mb-10">Habilidades</h1>
        <div class="d-flex flex-column flex-md-row justify-space-around align-sm-center mx-5 my-5 ">
            <v-row justify="center" align="center" no-gutters>
                <v-col
                    class="d-flex justify-center align-center"
                    v-for="(icon, index) in icons" :key="index"
                >
                    <v-card  
                        class="card-skill d-flex flex-column  justify-center my-5 "
                        width="150px"
                    >
                        <v-icon
                        class="m-6"
                        size="60"
                        color="white darken-2"
                        id="icon"
                        >
                            {{ icon.icon}}
                        </v-icon>
                        <p class="white--text text-center" > {{ icon.name }} </p>
                    </v-card>
                </v-col>
            </v-row>
        </div>


    
    </div>
</template>

<script>
export default {
    name: 'skill-dev',
    data() {
        return {
            icons: [
                {
                    name: 'HTML5',
                    icon: 'mdi-language-html5'
                },
                {
                    name: 'CSS 3',
                    icon: 'mdi-language-css3'
                },
                {
                    name: 'VUETIFY',
                    icon: 'mdi-vuetify'
                },
                {
                    name: 'JavaScript',
                    icon: 'mdi-language-javascript'
                },
                {
                    name: 'Bootstrap',
                    icon: 'mdi-bootstrap'
                },
                {
                    name: 'Sass',
                    icon: 'mdi-sass'
                },
                {
                    name: 'Mysql',
                    icon: 'mdi-database-search'
                },                
            ]

            
            
        }
    },
}
</script>

<style scoped>

    div{
        background-color: #1f1f1f;
    }
    .card-skill{
        background-color: #2A2929;
    }
    #icon{
        padding: 10px 25px;


    }
    i{
        font-size: 200px;
    }

</style>