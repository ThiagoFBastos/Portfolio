<template>
    <div class = "mt-2">
        <h3>Projetos</h3>
        <div v-for = "project in projects" class = "border-bottom mb-2 box">
           <a :href = "project.link" target = "__blank">
           <h5>{{project.title}}</h5>
            <p>{{project.description}}</p>
            <div>
                <span v-for = "skill in project.skills" class="mx-1 badge rounded-pill bg-dark text-light"># {{skill}}</span> 
            </div>
           </a>
        </div>
    </div>
</template>


<style scoped>
a {
    text-decoration: none;
    color: black;
}

.box {
    width: 400px;
}

.box:hover {
    background-color: rgba(0, 0, 0, 0.1);
}
</style>

<script>

    export default {
        name: 'Projects',
        components: {},
        data() {
            return {
                'projects': [
                    {
                       title: ' Linkedin BOT',
                       description: 'Bot de vagas no Linkedin para desenvolvedores.A partir de palavras-chave préviamente coletadas e de outros parâmetros para filtrragem.',
                       skills: ['python', 'postgresql', 'pandas', 'pyscopg2', 'docker', 'pandas', 'scikit-learn'],
                       link: 'https://github.com/ThiagoFBastos/Linkedin-BOT'
                    },
                    {
                        title: ' Repo Code',
                        description: 'Repositório local para guardar códigos ou buscá-los facilmente feito com Django.',
                        skills: ['HTML5', 'CSS3', 'django', 'sqlite'],
                        link: 'https://github.com/thiagofbastos/Repo-Code'
                    },
                    {
                        title: ' TodoList',
                        description: 'site para criar todo list feito com django.',
                        skills: ['python', 'django', 'sqlite'],
                        link: 'https://github.com/thiagofbastos/TodoList'
                    },
                    {
                        title: 'Closest String Problem',
                        description: 'heurísticas para o problema closest string.',
                        skills: ['c++', 'multithreading'],
                        link: 'https://github.com/thiagofbastos/closest-string-problem'
                    },
                    {
                        title: 'crawler_twitter',
                        description: 'crawler/bot de tweets do twitter usando selenium e beautifulsoup.',
                        skills: ['python', 'selenium', 'beautifulsoup'],
                        link: 'https://github.com/thiagofbastos/crawler_twitter'
                    },
                    {
                        title: 'SOS Board Game',
                        description: 'SOS board game em C++ (Gtkmm3.0)',
                        skills: ['c++', 'gtkmm'],
                        link: 'https://github.com/ThiagoFBastos/SOS-Board-Game'
                    },
                    {
                        title: ' tic tac toe',
                        description: 'tic tac toe - minimax ',
                        skills: ['c++', 'sdl'],
                        link: 'https://github.com/ThiagoFBastos/tic_tac_toe'
                    },
                    {
                        title: '3-admissibility',
                        description: 'gerador de grafos 3-admissíveis',
                        skills: ['c++', 'multithreading'],
                        link: 'https://github.com/ThiagoFBastos/3-admissibility'
                    },
                    {
                        title: 'Portifólio',
                        description: 'Site com vue puro para apresentar meus portifólios e falar um pouco sobre mim ',
                        skills: ['vuejs', 'javascript', 'nodejs'],
                        link: 'https://github.com/ThiagoFBastos/Portifolio'          
                    },
                    {
                        title: 'moMus',
                        description: 'Estudando Node.js, Express e Sequelize',
                        skills: ['nodejs', 'javascript', 'mysql', 'HTML5', 'CSS3', 'express', 'sequelize'],
                        link: 'https://github.com/ThiagoFBastos/moMus'
                    },
                    {
                        title: 'Isotree',
                        description: 'algoritmo para encontrar árvores não rotuladas ',
                        skills: ['c++', 'multithreading'],
                        link: 'https://github.com/ThiagoFBastos/isotree'
                    }
                ]
            }
        }
    }
</script>
