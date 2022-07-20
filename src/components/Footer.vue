<template>
    <div>
        <v-footer  padless>
            <v-card flat tile width="100%" class="indigo lighten-1 text-center">
                <v-card-text>
                    <v-btn v-for="(icon, index) in icons" :key="index" class="mx-4" icon>
                        <a :href="icon[1]">
                            <v-icon size="24px">
                                {{ icon[0] }}
                            </v-icon>
                        </a>
                    </v-btn>
                </v-card-text>

                <v-divider></v-divider>

                <v-card-text class="white--text">
                    {{ new Date().getFullYear() }} — <strong>Sergio Sepulveda</strong>
                </v-card-text>
            </v-card>
        </v-footer>
    </div>
</template>

<script>
export default {
    name: 'footer-me',
    data() {
        return {
            icons: [
                ['mdi-home', '#container'],
                ['mdi-email', 'mailto: contacto@penti2s.com'],
                
            ],
        }
    },

}
</script>

<style scoped>
a{
    text-decoration: none;
}
</style>