<template>
    <section class="px-8 py-12">
        <div class="grid grid-cols-2 gap-3">
            <CardStack  img="/Typescript.png" tecnologia="Typescript"/>
            <CardStack  img="/Node.png" tecnologia="NodeJs"/>
            <CardStack  img="/Vue.png" tecnologia="VueJs"/>
            <CardStack  img="/PHP.png" tecnologia="PHP"/>
            <CardStack  img="/Laravel.png" tecnologia="Laravel"/>
            <CardStack  img="/javaScript.png" tecnologia="JavaScript"/>
            <CardStack  img="/Nest.png" tecnologia="NestJs"/>
            <CardStack  img="/MySQL.png" tecnologia="MySQL"/>
            <CardStack  img="/Oracle.png" tecnologia="Oracle"/>
            <CardStack  img="/Mongo.png" tecnologia="MongoDB"/>
        </div>
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