<template>
    <section class="px-8 py-12 lg:px-44 2xl:px-96">
        <h1 class="text-white text-xl lg:text-4xl font-bold text-center mb-12"><span class="text-[#27AE60] font-bold">{{ '<' }}</span> Projetos <span class="text-[#27AE60] font-bold">{{ '/>' }}</span></h1>

        <div class="grid lg:grid-cols-2 gap-3">
            <CardProjetos titulo="Portfólio" descricao="Projeto de portfólio" github="https://github.com" deploy="https://github.com" />
            <CardProjetos titulo="Portfólio" descricao="Projeto de portfólio" github="https://github.com" deploy="https://github.com" />
            <CardProjetos titulo="Portfólio" descricao="Projeto de portfólio" github="https://github.com" deploy="https://github.com" />
            <CardProjetos titulo="Portfólio" descricao="Projeto de portfólio" github="https://github.com" deploy="https://github.com" />
        </div>

    </section>
</template>

<script>
import CardProjetos from './CardProjetos.vue';

export default {
    name: 'App',
    components: {
        CardProjetos
    }
}

</script>