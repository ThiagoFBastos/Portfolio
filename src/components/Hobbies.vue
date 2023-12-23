<template>
    <div>
        <h3>Competitive Programming</h3>

        <div v-for = "OJ in OJs" class = "row">
            <div class = "col col-sm-1">
                <img :src = "OJ.logo" class = "img img-thumbnail">
            </div>
            <div class = "col">
                <h5>{{OJ.site}}</h5>
                Usuário: <span>{{OJ.profile}}</span> <br>
                Link do Site: <a :href = "OJ.url" target = "__blank">{{OJ.url}}</a> <br>
                Link do Perfil: <a :href = "OJ.profile_link" target = "__blank">{{OJ.profile_link}}</a> <br>
            </div>
        </div>
    </div>
</template>

<script>
     export default {
        name: 'Hobbies',
        components: {},
        data() {
             return {
                OJs : [
                    {
                        site: 'Codeforces',
                        url: 'https://codeforces.com',
                        logo: 'codeforces.png',
                        profile: 'thiago_bastos',
                        profile_link: 'https://codeforces.com/profile/thiago_bastos'                    
                    },
                    {
                        site: 'Atcoder',
                        url: 'https://atcoder.jp/',
                        logo: 'atcoder.webp',
                        profile: 'thiago_bastos',
                        profile_link: 'https://atcoder.jp/users/thiago_bastos'                    
                    },
                    {
                        site: 'Codechef',
                        url: 'https://www.codechef.com/', 
                        logo: 'codechef.webp',  
                        profile: 'far_from_tle',
                        profile_link: 'https://www.codechef.com/users/far_from_tle'
                    }
                ]
            }
        }
    }
</script>

<style scoped>

</style>
