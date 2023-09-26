<template>
    <section id="sobre" class="px-8 py-12 lg:px-44 2xl:px-96 items-center headline">
        <div class="block border p-4 hover:bg-[#0e0e12] cursor-pointer border-white/10 rounded-lg">
            <h1 class="text-[#27AE60] font-bold mb-4">SOBRE MIM</h1>
            <p class=" text-white">
                Sou um Desenvolvedor Full Stack, tenho conhecimentos em TypeScript, NodeJS, Vuejs , PHP e Laravel, com habilidades para criar aplicações front-end e back-end eficientes e de alta qualidade. Tenho experiência em desenvolvimento de aplicações web, utilizando metodologias ágeis e práticas de desenvolvimento modernas. <br> <br>

                Meu objetivo é aplicar minha experiência e habilidades em projetos desafiadores, contribuindo para o sucesso de uma empresa inovadora e em constante crescimento. Estou sempre buscando aprimorar meu conhecimento técnico e me manter atualizado com as últimas tendências e melhores práticas de desenvolvimento. <br> <br>

                Sinta-se à vontade para entrar em contato comigo para discutir oportunidades de colaboração. Estou ansioso para fazer parte de uma equipe inovadora e impulsionar o sucesso dos projetos de forma eficaz. <br> <br>
            </p>
        </div>
    </section>
</template>

<script>
export default {
    created() {
        ScrollReveal().reveal('.headline');
    }
}

</script>