<template>
    <div>

    </div>
</template>

<script>

let est1 = {
    codigo: 1,
    nombre: 'Lucas Mera',
    descripcion: 'Lorem ipsum dolor sit amet, consectetur adipiscing',
    rol: 'Desarrollador backend',
    image: 'path/to/image'
    };

    export default {
        name: "TeamCard",
        props: ['member'],
        data(){
            return{
                estudiante1:est1,
                }
            }
    }
</script>

<style scoped>

</style>
