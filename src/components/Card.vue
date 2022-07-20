<template>
    <v-main class="mb-10">
        <v-card
            class="mx-auto my-10"
            max-width="300"
            id="imgCard"
            elevation="9"
        >
                    <v-img
                        src="@/assets/Edit2Web.jpg"
                        height="200px"
                    ></v-img>
                    <v-row > 
                        <v-col sm="4" md="4" class="d-flex justify-center align-center">
                            <v-img
                                class="my-2"
                                height="80"
                                width="80"
                                src="@/assets/html.png"
                            ></v-img>
                        </v-col>
                        <v-col sm="4" md="4" class="d-flex justify-center align-center">
                            <v-img
                                height="80"
                                width="80"
                                src="@/assets/jsicon.png"
                            ></v-img>
                        </v-col>
                        <v-col sm="4" md="4" class="d-flex justify-center align-center">
                            <v-img
                                height="80"
                                width="80"
                                src="@/assets/vuejs.png"
                            ></v-img>
                        </v-col>
                    </v-row>

                </v-card>
    </v-main>
</template>

<script>
export default {
    name: 'card-me'
}
</script>

<style>
    h2{
        padding-top: 50px;
        text-align: center;
    }
    #imgCard{
        padding: 10px;
    }
</style>