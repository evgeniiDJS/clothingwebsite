<template>
    <div class="v-main-wrapper">
        <p>{{ title }}</p>
        <v-catalog />
    </div>
</template>

<script>
    import vCatalog from './v-catalog.vue'

    export default {
        name: 'v-main-wrapper',
        components: {
            vCatalog
        },
        props: {},
        data() {
            return {
                title: 'Main Wrappers!'
            }
        },
        computed: {},
        methods: {},
        watch: {},
    }
</script>

<style>
    .v-main-wrapper {
        max-width: 900px;
        margin: 0 auto;
    }
</style>