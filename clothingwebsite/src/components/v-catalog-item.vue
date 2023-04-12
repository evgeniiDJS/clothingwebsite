<template>
    <div class="v-catalog-item">
        <img class="v-catalog-item__image" src="../assets/crossfashion_567d68020065c6f6f1dbb9c0eb789375.jpg" alt="img">
        <p class="v-catalog-item__name">{{ product_data.name }}</p>
        <p class="v-catalog-item__price">Price: {{ Math.round(product_data.price) }} LT</p>
        <button 
            class="v-catalog-item__add_to_cart_btn btn" 
            @click="sendDataToParent"
            >Add to cart</button>
    </div>
</template>

<script>
    export default {
        name: 'v-catalog-item',
        components: {},
        props: {
            product_data: {
                type: Object,
                default() {
                    return {}
                }
            }
        },
        data() {
            return {
                title: 'v-catalog-item'
            }
        },
        computed: {},
        methods: {
            sendDataToParent() {
                this.$emit('sendDataToParent', this.product_data.article)
            }
        },
        watch: {},
    }
</script>

<style lang="scss">
    .v-catalog-item__image {
        width: 100px;
    }

    .v-catalog-item{
        display: block;
        width: 250px;
        flex-basis: 25%;
        box-shadow: 0 0 8px 0 #e0e0e0;
        padding: 16px;
        margin-bottom: 16px;
    }
</style>