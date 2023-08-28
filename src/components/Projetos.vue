<template>
    <section id="projetos" class="px-8 py-12 lg:px-44 2xl:px-96">
        <h1 class="text-white text-3xl lg:text-4xl font-bold text-center mb-12"><span class="text-[#27AE60] font-bold">{{ '<' }}</span> Projetos <span class="text-[#27AE60] font-bold">{{ '/>' }}</span></h1>

        <div class="grid lg:grid-cols-2 gap-3">
            <CardProjetos 
                titulo="SmartHome" 
                descricao="Landing page SmartHome" 
                imagem="SmartHome.png" 
                github="https://github.com/tonyalbert/HomeSmart-vue" 
                deploy="https://home-smart-vue.vercel.app/" 
            />

            <CardProjetos 
                titulo="Miles Morales page" 
                descricao="Miles Morales landing page" 
                imagem="miles.png" 
                github="https://github.com/tonyalbert/miles-morales-page" 
                deploy="https://miles-morales-page.vercel.app/" 
            />

            <CardProjetos 
                titulo="Portfólio" 
                descricao="Projeto de portfólio" 
                imagem="portfolio.png" 
                github="https://github.com" 
                deploy="https://github.com" 
            />

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