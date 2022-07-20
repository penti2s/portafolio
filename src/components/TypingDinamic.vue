<template>
    <div>
        <VueTyper  class="text-h5" :text='subtext' />
    </div>
</template>

<script>
import { VueTyper } from 'vue-typer'
export default {
    name: 'typing-dinamic',
    components: {
        VueTyper,
    },
    data() {
        return {
            subtext: [
                'Front-end Developer',
                'Desarrollador Web'
            ]
        }
    },
}
</script>

<style scoped>

</style>