<template>
  <TheHeader />
  <Hero />
</template>

<script>
import Hero from './components/Hero.vue';
import TheHeader from './components/TheHeader.vue';

export default {
  name: 'App',
  components: {
    TheHeader,
    Hero
  }
}

</script>