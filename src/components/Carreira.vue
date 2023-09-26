<template>
    <section id="projetos" class="px-8 py-12 lg:px-44 2xl:px-96">
        <h1 class="text-white text-3xl lg:text-4xl font-bold text-center mb-12"><span class="text-[#27AE60] font-bold">{{ '<' }}</span> Carreira <span class="text-[#27AE60] font-bold">{{ '/>' }}</span></h1>

        <div class="grid md:grid-cols-2 gap-3">

            <CardTrabalho
            periodo="Maio de 2023 - Atualmente"
            nome="Lince Web"
            funcao="Desenvolvedor Full Stack"
            descricao="Desenvolvimento de plataformas de delivery utilizando Laravel PHP e Vue.js. Colaboração
            com a equipe de design para criar interfaces envolventes e amigáveis. Arquitetura e
            desenvolvimento de recursos robustos no back-end com Laravel PHP. Implementação de
            componentes front-end interativos usando Vue.js. Resolução de bugs e otimização de
            desempenho no cliente e servidor. Participação ativa em sprints ágeis, reuniões de equipe e
            revisões de código."
            :tecnologias=tecnologiasLince
            />

            <CardTrabalho
            nome="Grupo São Roque"
            periodo="Novembro de 2022 - Maio de 2023"
            funcao="Desenvolvedor - Estágio"
            descricao="Responsável por construir APIs escaláveis e eficientes, que oferecem suporte a
            diversas operações de negócios. Além disso, trabalho com a integração de bancos
            de dados, garantindo que os dados sejam armazenados e gerenciados de forma
            adequada e segura."
            :tecnologias=tecnologiasSaoRoque
            />


        </div>
    </section>
</template>

<script setup>
import { ref } from 'vue';
import CardTrabalho from './CardTrabalho.vue';
import php from '../../public/PHP.png';
import laravel from '../../public/Laravel.png';
import javascript from '../../public/javaScript.png';
import typescript from '../../public/Typescript.png';
import mysql from '../../public/MySQL.png';
import oracle from '../../public/Oracle.png';

const tecnologiasLince = ref([
    { 
        img: php,
        nome: 'PHP',
    },
    {
        img: laravel,
        nome: 'Laravel',
    },
    {
        img: javascript,
        nome: 'JavaScript',
    },
    {
        img: typescript,
        nome: 'TypeScript',
    },
    {
        img: mysql,
        nome: 'MySQL',
    }
])

const tecnologiasSaoRoque = ref([
    {
        img: javascript,
        nome: 'JavaScript',
    },
    {
        img: typescript,
        nome: 'TypeScript',
    },
    {
        img: oracle,
        nome: 'oracle',
    }
])

</script>