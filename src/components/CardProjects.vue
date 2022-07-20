<template>
    <v-card class="mx-auto my-15" id='card-project' @click="dialog3 = true">
        <v-sheet elevation="3" class="mx-2 my-2">
            <v-img class="white--text align-end ma-3" height="200px" :src="data.img">>
            </v-img>
        </v-sheet>
        <h3 class="text-center mb-1 mb-10 mt-5"> {{ data.name}}</h3>
        <v-row justify="center">
            <v-dialog v-model="dialog3" max-width="800px">
                <v-card>
                    <v-card-title>
                        <span>{{data.name}}</span>
                        <v-spacer></v-spacer>
                    </v-card-title>

                    <v-container>
                        <v-carousel v-model="model">
                            <v-carousel-item v-for="(item, index) in data.carrouseImg" :key="index">
                                <v-sheet height="100%" tile>
                                    <v-img contain max-height="100%" max-width="100%" :src='item'></v-img>
                                </v-sheet>
                            </v-carousel-item>
                        </v-carousel>

                    </v-container>
                    <p class="px-5">{{ data.description }}</p>
                    <p class="px-5">Repositorio Link: <a target="_blank" :href="data.linkRepo">{{ data.linkRepo }}</a></p>
                    <v-card-actions>
                        <v-btn color="primary" text @click="dialog3 = false">
                            Close
                        </v-btn>
                    </v-card-actions>
                </v-card>
            </v-dialog>
            <v-dialog id="modal-card" open-on-click :z-index="zIndex" :value="overlay" opacity="1">
                <v-card class="d-flex-inline">
                    <v-container>
                        <v-carousel v-model="model">
                            <v-carousel-item v-for="(color, i) in colors" :key="color">
                                <v-sheet :color="color" height="100%" tile>
                                    <v-row class="fill-height" align="center" justify="center">
                                        <div class="text-h2">
                                            Slide {{ i + 1 }}
                                        </div>
                                    </v-row>
                                </v-sheet>
                            </v-carousel-item>
                        </v-carousel>

                    </v-container>
                    <h2 class="py-2">{{ data.name }}</h2>
                    <p class="px-5">{{ data.description }}</p>
                    <p class="px-5">Repositorio Link: {{ data.linkRepo }}</p>
                    <p class="px-5">Demo Link: {{ data.linkDemo }}</p>
                </v-card>
            </v-dialog>
        </v-row>
    </v-card>
</template>

<script>
export default {
    name: "card-project",
    props: {
        data: Object,
        img: String,
    },
    data() {
        return {
            overlay: false,
            zIndex: 0,
            model: 0,
            dialog3: false,
            colors: [
                'primary',
                'secondary',
                'yellow darken-2',
            ],
        }
    },
};
</script>

<style scoped>
#card-project {
    transition: box-shadow 0.3s ease-in-out;
    border-radius: 0px;
    border: 1px solid #ccc;
    max-width: 400px;
}

#card-project:hover {
    box-shadow: 7px 7px 25px rgba(0, 0, 0, 0.8);
}

#modal-card {
    width: 80vw;
}
</style>