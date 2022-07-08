<template>
    <v-main >
        <v-row id="container">
            <v-col class="d-flex flex-column justify-center align-center">
                    <v-icon
                        large
                        color="blue darken-2"
                    >
                        mdi-laptop
                    </v-icon>
                    <p> Sergio Sepulveda </p>
            </v-col>
        </v-row>
    </v-main>
</template>

<script>
export default {
    name: 'header-components',
}
</script>

<style scoped>
    *{
        box-sizing: border-box;
        
    }
    #container {
        background: #3F51B5;
        height: 100vh;
    }
    #center{

    }


</style>