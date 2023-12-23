
<template>
    <div>
        <h1>{{nome}}</h1>
        <p>{{description}}</p>
    </div>
</template>

<script>
    export default {
        name: 'Description',
        data() {
            return {
                nome: 'Thiago Bastos',
                description: 'Técnico em Programação pelo Colégio Pedro II e Bacharel em Ciência da Computação pela UFRRJ. Atualmente desenvolvo aplicações com: C/C++, Python, Javascript, C# e SQL. Sou apaixonado por programação competitiva que é uma esporte mental no qual os praticadores resolvem desafios lógicos e matemáticos com programação.',
            }
        }
    }
</script>

<style scoped>
p, h1 {
    color: white;
}
</style>
