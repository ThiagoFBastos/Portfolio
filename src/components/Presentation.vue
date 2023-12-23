<template>
    <div class = "container-fluid">
        <div class = "presentation-top">
            <div class = "row">
                <div class = "col text-center">
                    <img class = "rounded-circle" id = "photo" src = "../assets/img/40869714.jpg">
                </div>
                <div class = "col align-items-center justify-content-center mt-5">
                    <Description/>
                    <Skills/>
                </div>
            </div>
        </div>
        <Formation/>
        <Experiences/>
        <Hobbies/>
        <Projects/>
        <Contact/>
    </div>
</template>

<style scoped>
#photo {
    max-height: 300px;
    max-width: 300px;
}
</style>

<script>
    import Description from './Description.vue'
    import Skills from './Skills.vue'
    import Formation from './Formation.vue'
    import Experiences from './Experiences.vue'
    import Hobbies from './Hobbies.vue'
    import Projects from './Projects.vue'
    import Contact from './Contact.vue'

    export default {
        name: 'Presentation',
        components: {
            Description,
            Skills,
            Formation,
            Experiences,
            Hobbies,
            Projects,
            Contact
        },
        data() {
             return {
                nome: 'Thiago Bastos'     
            }
        }
    }
</script>

<style scoped>
.presentation-top {
    background-image: url('background.png');
	background-repeat: no-repeat;
	background-position: center;
	background-size: cover;
    background-color: rgba(0, 0, 0, 0.8)
}

</style>
