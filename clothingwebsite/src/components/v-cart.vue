<template>
    <div class="v-cart">
        <p>{{ title }}</p>
    </div>
</template>

<script>
    export default {
        name: 'v-cart',
        components: {},
        props: {},
        data() {
            return {
                title: 'v-cart'
            }
        },
        computed: {},
        methods: {},
        watch: {},
    }
</script>

<style>
    .v-cart{
        display: flex;
        justify-content: center;
        align-items: center;
        max-width: 900px;
        margin: 0 auto;
    }
</style>