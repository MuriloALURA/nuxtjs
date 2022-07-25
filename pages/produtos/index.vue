<template>
        <div>
            <h1 class="text-lg font-bold" >Produtos</h1>
            <nuxt-link to="/produtos/produto-a">Produtos A</nuxt-link>   
            <nuxt-link to="/produtos/produto-b">Produtos B</nuxt-link>   

            <br>
            <br>

            <div v-for="product in products" :key="'product.id'">
                {{product.title}}
            </div>

            <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.</p>
        </div>
</template>
<script>
export default {
    name: '',

    data() {
        return {
        };
    },

    async asyncData({$axios}) {
        const products = await $axios.$get('https://jsonplaceholder.typicode.com/users?_limit=3');
        return{
            products,
        }
    },

    methods: {},
    
}
</script>
<style>
    
</style>