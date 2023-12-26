
<template>
    <div>
        <h3>Linguagens de Programação</h3>
        <div>
            <span v-for = "language in languages" class="mx-1 badge rounded-pill bg-light text-dark"># {{language}}</span> 
        </div>
    </div>
    <div class = "mt-2">
        <h3>Banco de dados</h3>
        <div>
            <span v-for = "database in databases" class="mx-1 badge rounded-pill bg-light text-dark"># {{database}}</span> 
        </div>
    </div>
    <div class = "mt-2">
        <h3>Backend</h3>
        <div>
            <span v-for = "backend in backends" class="mx-1 badge rounded-pill bg-light text-dark"># {{backend}}</span> 
        </div>
    </div>
   <div class = "mt-2">
        <h3>Frontend</h3>
        <div>
            <span v-for = "frontend in frontends" class="mx-1 badge rounded-pill bg-light text-dark"># {{frontend}}</span> 
        </div>
    </div>
</template>

<script>
    export default {
        name: 'Skills',
        data() {
            return {
                languages: ['C/C++', 'Pyrhon', 'Javascript', 'C#'],
                databases: ['SQL', 'PostgresSQL', 'MySQL'],
                backends: ['Django', 'Nodejs', 'Sequelize'],
                frontends: ['HTML5', 'CSS3']  
            }
        }
    }
</script>

<style scoped>
h3 {
    color: white;
}
</style>
