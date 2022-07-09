<template>
    <v-main id="container" > 
        <v-row justify="center">
            <v-col cols="12" xs="12" sm="12" md="12"> 
                <h1 class="text-center mt-5"> Proyectos </h1> 
            </v-col>
            <v-col cols="3" xs="3">
                Proyecto 1 
            </v-col>
            <v-col cols="3" xs="3">
                Proyecto 2 
            </v-col>
            <v-col cols="3" xs="3">
                Proyecto 3 
            </v-col>
        </v-row>
    </v-main>
</template>

<script>
export default {
    name: 'project-dev'
}
</script>

<style scoped>
    *{
        box-sizing: border-box;
        
    }
    #container {
        background: #3F51B5;
        height: 25vh;
    }
</style>