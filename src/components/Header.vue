<template>
    <v-row id="container" no-gutters class="d-flex flex-rown align-center justify-center indigo lighten-1">
        <v-col class="d-flex flex-column align-center">

                <v-icon size="100" color="blue darken-2">
                    mdi-laptop
                </v-icon>
                <h1 class="mb-0">Sergio Sepulveda</h1>
                <TypingDinamic class="pt-0" />
        </v-col>
    </v-row>

</template>

<script>
import TypingDinamic from './TypingDinamic.vue'
export default {
    name: 'header-components',
    components: {
        TypingDinamic,
    }
}
</script>

<style scoped>
* {
    box-sizing: border-box;
}

#container {
    min-height: 40%;
    max-height: 80%;
}

span{
    display: block;
    font-family: monospace;
    white-space: nowrap;
    border-right: 4px solid;
    width: 16ch;

    animation: typing 2s steps(16), blink .5 infinite step-end alternate;
    overflow: hidden;
}

@keyframes typing {
    from { width: 0 }
}
@keyframes blink {
    50% {border-color: transparent;}
}
</style>