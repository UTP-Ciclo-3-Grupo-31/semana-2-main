<template>
    <div class="container" id="estudiantes">
    <h2>PRUEBA</h2>
        <div class="row">
            <h2>{{estudiantes.nombre}}</h2>
            Codigo: {{estudiantes.codigos}}
        </div>
    </div>
</template>

<script>

    export default {
        name: "TeamCard",
        props: ['member'],
        data(){
            return{
                estudiantes:[{
                    codigo: 1,
                    nombre: 'Sergio Vargas',
                    descripcion: "Programador,vive en BogotÃ¡, le gusta Jugar con electrÃ³nica, volar drones y le apasionan las motos",
                    rol: 'Desarrollador backend',
                    image: "img/Avatar1.png"
                    },
                    {
                        codigo: 2,
                        nombre: 'Diego Lipiz',
                        descripcion: "Ingeniero electricista de la Universidad Industrial de Santander, nacido en Bucaramanga actualmente vive en BogotÃ¡, le gustan las caminatas por el campo y jugar minecraft con su hija.",
                        rol: 'Desarrollador backend',
                        image: "img/Avatar2.png"
                    },
                    {
                        codigo: 3,
                        nombre: 'Jose del Valle',
                        descripcion: "Ingeniero de Control de la Universidad Nacional de Colombia, nacido en ItagÃ¼Ã­ vive actualmente en MedellÃ­n le gusta jugar vÃ­deo juegos.",
                        rol: 'Desarrollador backend',
                        image: "img/Avatar3.png"
                    }, 
                    {
                        codigo: 4,
                        nombre: 'Esteban DurÃ¡n',
                        descripcion: "Ingeniero QuÃ­mico de la Universidad de Antioquia, vive en MedellÃ­n, le gusta hacer deporte, leer y el cine.",
                        rol: 'Desarrollador backend',
                        image: "img/Avatar4.png"
                    },
                    {
                        codigo: 5,
                        nombre: 'Engie Lorena Hernandez',
                        descripcion: "Bogotana, tecnologa en gastronomia de la Universitaria Agustiniana, creativa, vive en busqueda constante de conocimiento, casada tiene una hija, apasionada por el arte, vive en la ciudad de Bogota y le gusta explorar rincones gastronomicos poco conocidos de esta ciudad.",
                        rol: 'Desarrollador frontend',
                        image: "img/Avatar5.png"
                    }],
                }
            }
    }
</script>

<style scoped>

</style>
