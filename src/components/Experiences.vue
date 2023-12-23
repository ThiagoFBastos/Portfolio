<template>
    <div class = "mt-5 rounded">
        <h3>Experiências</h3>
        <div v-for = "e in experiences" class = "row">
            <div class = "col col-sm-1 text-center">
               <img :src = "e.img" class = "img img-thumbnsil img-fluid">
            </div>
            <div class = "col">
                <h4>{{e.title}}</h4>
                <span>{{e.from}} - {{e.to}}</span> <br>
                <span>{{e.location}}</span> <br>
                <span>{{e.entity}}</span> <br>
                <span>{{e.role}}</span> <br>
                <p>{{e.description}}</p>
            </div>
        </div>
    </div>
</template>

<script>
     export default {
        name: 'Experiences',
        components: {},
        data() {
             return {
                experiences: [
                    {img: 'cnpq.jpg', location: 'Rio de Janeiro, Brasil', entity: 'CNPq', title: 'Iniciação Científica', role: 'Bolsista de Iniciação científica', from: '03/2022', to: '08/2022', 'description': 'Projeto que visava o descobrimento de certas propriedades de uma certa classe de grafos, da teoria dos grafos, através de algoritmos implementados em C++ e usando multithreading, estruturas de dados bem como outros algoritmos clássicos presentes na literatura afim de serem usados para descobrir uma maneira de caracterizar essa classe de grafos.'},
                    {img: 'faperj.jpg', location: 'Rio de Janeiro, Brasil',  entity: 'FAPERJ', title: 'Iniciação Científica', role: 'Bolsista de Iniciação científica', from : '03/2015', to: '12/2017', 'description': 'Projeto que visava o descobrimento de certas propriedades de uma certa classe de grafos, da teoria dos grafos, através de algoritmos implementados em C++ e usando multithreading, estruturas de dados bem como outros algoritmos clássicos presentes na literatura afim de serem usados para descobrir uma maneira de caracterizar essa classe de grafos.'},
                    {img: 'pedroii.jpg', location: 'Rio de Janeiro, Brasil', entity: 'Colégio Pedro II', title: 'Monitoria de linguagem de programação', role: 'Monitor da disciplina C#', from: '05/2017', to: '12/2017', description: ' Auxiliava nas duvidas dos alunos referente a disciplina e resolvia questões de C# com a turma;'}                
                ]
            }
        }
    }
</script>

<style scoped>

</style>

