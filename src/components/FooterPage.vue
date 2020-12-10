<template>
    <footer class = "footer">
        <div>
            <h4><strong>Descripción del sitio web</strong></h4>
            <p> Este es un desarrollo Web creado por los estudiantes del grupo 31,<br> 
                dentro del marco del modulo 3 del proyecto Misión Tic 2022, con el<br> 
                cual se pretende mostrar las habilidades obtenidas durante la semana<br>
                2 de dicho Modulo. <br> <br> 

                <a href="https://github.com/UTP-Ciclo-3-Grupo-31/semana-2-main">https://github.com/UTP-Ciclo-3-Grupo-31/semana-2-main</a>
            </p>

            
        </div>
        <div>
            <h4><strong>Integrantes del Equipo 31</strong></h4>
            <div class = "footer">

                <div>
                    <p> Engie Lorena Hernandez Lopez &nbsp; &nbsp; <br>
                        Diego Mauricio Lipez Lipez <br>
                        Jose  Fernando Del Valle Henao <br> 
                        Sergio Vargas <br>
                        Esteban Durán Rojas
                    </p>
                </div>

                <div>
                    <p> 
                        <a href="mailto:engielhernandezl@hotmail.com"> engielhernandezl@hotmail.com </a> <br>
                        <a href="mailto:diegolipez@gmail.com"> diegolipez@gmail.com </a> <br>
                        <a href="mailto:aleriuz@gmail.com"> aleriuz@gmail.com </a> <br> 
                        <a href="mailto:sergiovargas9@gmail.com"> sergiovargas9@gmail.com </a>  <br>
                        <a href="mailto:estebanduranr@hotmail.com"> estebanduranr@hotmail.com </a> 
                    </p>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
    export default {
        name: "FooterPage",
        props: ['FooterPage'],
        data(){
            return{
               
                }
            }
    }
</script>

<style scoped>
.footer{
    background-color: #b4b7be;
    color: black;
    display: flex;
    justify-content: space-evenly;
    align-items: center;
}
</style>
