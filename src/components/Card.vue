<template>
    <v-main>
        <v-card
            class="mx-auto"
            max-width="300"
            id="imgCard"
            elevation="9"
        >
                    <v-img
                        src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
                        height="200px"
                    ></v-img>
                    <v-card-title>
                    Top western road trips
                    </v-card-title>

                    <v-card-subtitle>
                    <v-row>
                        <v-col sm="4" md="4">
                            <v-img
                                max-height="191"
                                max-width="80"
                                src="@/assets/vue-icon.png"
                            ></v-img>
                        </v-col>
                        <v-col sm="4" md="4">
                            <v-img
                                max-height="191"
                                max-width="80"
                                src="@/assets/vue-icon.png"
                            ></v-img>
                        </v-col>
                        <v-col sm="4" md="4">
                            <v-img
                                max-height="191"
                                max-width="80"
                                src="@/assets/vue-icon.png"
                            ></v-img>
                        </v-col>
                    </v-row>
                    </v-card-subtitle>
                    <v-spacer></v-spacer>
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