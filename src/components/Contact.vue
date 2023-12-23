<template>
    <div class = "mt-5">
        <div class = "container">
            <table class = "table">
                <thead>
                    <tr class = "text-center">
                        <th colspan = "2">Contato</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>Email</td>
                        <td>{{email}}</td>
                    </tr>
                    <tr>
                        <td>Celular</td>
                        <td>{{celular}}</td>
                    </tr>
                    <tr>
                        <td>Github</td>
                        <td><a :href = "github" target = "__blank">{{github}}</a></td>
                    </tr>
                    <tr>
                        <td>Linkedin</td>
                        <td><a :href = "linkedin" target = "__blank">{{linkedin}}</a></td>
                    </tr>
                </tbody>
            </table>
        </div>
    </div>
</template>

<style scoped>
    .container {
        max-width: 600px
    }
</style>

<script>
    export default {
        name: 'Presentation',
        data() {
             return {
                email: 'thiagobastos1705@gmail.com',
                celular: '(21) 99702-7654',
                github: 'https://github.com/ThiagoFBastos',
                linkedin: 'https://www.linkedin.com/in/thiago-bastos-845a691a6/'
            }
        }
    }
</script>
