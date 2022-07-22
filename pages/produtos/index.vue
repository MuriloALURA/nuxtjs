<template>
    <div>
        <div class="bg-gray-100">
            <div class="container mx-auto flex items-center space-x-4 h-10 mb-10">
                <nuxt-link to="/a-empresa">A empresa</nuxt-link>
                <nuxt-link to="/servicos">Serviços</nuxt-link> 
                <nuxt-link to="/produtos">Produtos</nuxt-link>                
            </div>
        </div>
    <div>
        <div class="container mx-auto">
            <h1 class="text-lg font-bold" >Produtos</h1>
            <nuxt-link to="/produtos/produto-a">Produtos A</nuxt-link>   
            <nuxt-link to="/produtos/produto-b">Produtos B</nuxt-link>   
            <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.</p>
        </div>
    </div>

    </div>
</template>
<script>
export default {
    
}
</script>
<style>
    
</style>