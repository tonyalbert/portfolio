<template>
    <section class="px-8 py-12 lg:px-44">
        
        <h1 class="text-white text-xl lg:text-4xl font-bold mb-6 text-center mb-12">Tecnologias</h1>
        <div class="grid grid-cols-2 lg:grid-cols-5 gap-3">
            <CardStack bdColor="4px solid #0385D2" img="/Typescript.png" tecnologia="Typescript"/>
            <CardStack bdColor="4px solid #64B749" img="/Node.png" tecnologia="NodeJs"/>
            <CardStack bdColor="4px solid #E0234E" img="/Nest.png" tecnologia="NestJs"/>
            <CardStack bdColor="4px solid #3FB27F" img="/Vue.png" tecnologia="VueJs"/>
            <CardStack bdColor="4px solid #35BEF8" img="/Tailwind.png" tecnologia="Tailwind"/>
            <CardStack bdColor="4px solid #7377AD" img="/PHP.png" tecnologia="PHP"/>
            <CardStack bdColor="4px solid #F72C1F" img="/Laravel.png" tecnologia="Laravel"/>
            <CardStack bdColor="4px solid #F7E018" img="/javaScript.png" tecnologia="JavaScript"/>
            <CardStack bdColor="4px solid #E47834" img="/MySQL.png" tecnologia="MySQL"/>
            <CardStack bdColor="4px solid #ED3237" img="/Oracle.png" tecnologia="Oracle"/>
        </div>
    </section>

    <section class="min-h-screen">

    </section>
</template>

<script>
import CardStack from './CardStack.vue';
import emblaCarouselVue from 'embla-carousel-vue'

export default {
    components: {
        CardStack
    },
    setup() {
      const [emblaNode] = emblaCarouselVue()
      return { emblaNode }
    }
}
</script>