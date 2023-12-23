<template>
    <div class = "mt-5 rounded">
        <h3>Formação</h3>
        <div v-for = "f in formation" class = "row">
            <div class = "col col-sm-1 text-center">
               <img :src = "f.img" class = "img img-thumbnsil img-fluidss">
            </div>
            <div class = "col">
                <h4>{{f.title}}</h4>
                <span>{{f.from}} - {{f.to}}</span> <br>
                <span>{{f.course}}</span> <br>
                <p>{{f.description}}</p>
            </div>
        </div>
    </div>
</template>

<script>
     export default {
        name: 'Formation',
        components: {},
        data() {
             return {
                formation: [
                    {img: 'ufrrj.jpg', title: 'UFRRJ', course: 'Bacharelado em Ciência da Computação', from: '03/2018', to: '09/2023', 'description': ' Curso de Bacharelado em Ciência da Computação do Instituto Multidisciplinar da Universidade Federal Rural do Rio de Janeiro, com sede no município de Nova Iguaçu pretende formar um profissional capaz de atuar em uma ampla gama de áreas e projetos. Com este objetivo, o profissional deverá considerar as possíveis diferenças de desenvolvimento e as diversidades técnicas, culturais e sociais. Adicionalmente, o profissional deverá refletir sobre sua prática profissional, suas atribuições, conhecer teorias e técnicas existentes, para capacitar-se a criar novas alternativas, assumindo um papel de agente produtor de conhecimentos'},
                    {img: 'pedroii.jpg', title: 'Colégio Pedro II', course: 'Curso técnico em Desenvolvimento de Sistemas', from : '03/2015', to: '12/2017', 'description': ' O curso técnico em Desenvolvimento de Sistemas forma profissionais capazes de desenvolver sistemas computacionais para web, desktop e dispositivos móveis em diversas linguagens de programação. Outras habilidades e competências desenvolvidas durante o curso envolvem a modelagem, implementação e manutenção de bancos de dados, além da elaboração e interpretação da documentação de sistemas.\nDurante os 3 anos do curso, o estudante participará de disciplinas nas áreas de programação, lógica, bancos de dados, desenvolvimento desktop, web e mobile, assim como processos de engenharia de software. Após a conclusão, os alunos podem atuar em diversas áreas da computação e, caso decidam seguir com a carreira no nível superior, estará muito bem preparado para dar continuidade aos estudos cursando Ciência da Computação, Sistemas de Informação e/ou Engenharias.'}
                ]
            }
        }
    }
</script>

<style scoped>

</style>

