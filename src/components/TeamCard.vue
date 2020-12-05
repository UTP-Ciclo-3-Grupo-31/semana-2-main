<template>
    <div class="card text-white bg-dark">
        <div class="d-flex justify-content-center pt-2">
            <img :src="member.image" alt="Fotografia Miembro">
        </div>
        <div class="card-body">
            <h3 class="card-title">{{member.nombre}}</h3>
            <p class="card-text">{{member.descripcion}}</p>
            <p class="card-text"><span>Rol: </span>{{member.rol}}</p>
            <p class="card-text"><span>Codigo: </span>{{member.codigo}}</p>
        </div>
    </div>
</template>

<script>

    export default {
        name: "TeamCard",
        props: {
            'member': Object
            }
    }
</script>

<style scoped>

</style>
