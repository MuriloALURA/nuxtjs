<template>
    <div>

            <pre>
                {{$fetchState}}
            </pre>

            <div v-if="$fetchState.pending">
                Carregando...
            </div>
            
            <div v-else>              
                <div v-for="service in services" :key="service.id"
                class="border-b border-gray-400 py-4">

                {{service.username}}
                </div>
            </div>
        
        <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.</p>
    </div>
</template>



<script>
export default {
    name: '',

    data() {
        return {
            services: []
        };
    },

    async fetch() {
        this.services = await this.$axios.$get('users?_limit=3');
            console.log(this);
        },

    methods: {},
    
}
</script>



<style>
    
</style>