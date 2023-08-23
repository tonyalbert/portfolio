<template>
  <div class="bg-[#09090B]">
    <TheHeader />
    <Hero />
    <Sobre />
    <Stack />
  </div>
</template>

<script>
import Hero from './components/Hero.vue';
import TheHeader from './components/TheHeader.vue';
import Sobre from './components/Sobre.vue';
import Stack from './components/Stack.vue';

export default {
  name: 'App',
  components: {
    Hero,
    TheHeader,
    Sobre,
    Stack
  }
}

</script>