<template>
    <v-main id="container">
        <v-row no-gutters>
            <v-col cols="12" sm="12" md="12" class="mt-10 mb-10">
                <h2 class="text-h4">Sobre Mi</h2>
            </v-col>
            <v-col cols="12" xs="12" sm="12" md="5">
                <Card />
            </v-col>
            <v-col cols="12" xs="12" sm="12" md="7" class="mt-10" >
                <v-card
                    id="header-container"
                    outlined
                    tile
                >
                    <v-card id="header-card"
                        outlined
                        tile
                    >
                        <div id="red" class="circle">
                        </div>
                        <div id="yellow" class="circle">
                        </div>
                        <div id="green" class="circle">
                        </div>
                    </v-card>
                    <div id="body-card" >
                        <h2 class="text-left"> Hola!!! </h2>
                        <div>
                            Lorem ipsum dolor sit amet consectetur adipisicing elit. Fugiat
                            blanditiis voluptatem explicabo similique earum expedita alias, 
                            nostrum, harum numquam necessitatibus a debitis
                            ut accusantium quisquam excepturi provident officiis animi error.
                        </div>
                    </div>

                </v-card>
            </v-col>
        </v-row>
    </v-main>
</template>

<script>
import Card from '@/components/Card.vue'
export default {
    name: 'about-me',
    components: {
        Card,
    }
}
</script>

<style scoped>
    *{
        box-sizing: border-box;
        margin: 0px;
        padding: 0px;
    }
    #container {
        height: 50vh;
    }
    h2{
        margin: 20px 20px 20px 0px;
    }
    .circle{
        display: inline-block;
        height: 15px;
        width: 15px;
        margin: 5px 5px;

    }
    #red{
        background-color: red;
        margin-left: 10px;
        border-radius: 50%;
    }
    #yellow{
        background-color: yellow;
        border-radius: 50%;
    }
    #green{
        background-color: green;
        border-radius: 50%;
    }
    #header-container{
        max-width: 90%;
        margin: 0px auto;
    }
    #header-card{
        background-color: #e8eaf660;
    }
    #body-card{
        display: flex;
        flex-direction: column;
        height: 200px;
        margin: 15px;
    }
</style>