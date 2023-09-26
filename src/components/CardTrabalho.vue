<template>
    <section >
        <div class="text-white bg-zinc-900/25 border border-zinc-800 p-8 rounded-md">

            <div class="mt-4">
                <div>
                    <h2 class="font-bold text-zinc-200 text-2xl mb-3">{{ nome }}</h2>
                    <p class="text-base text-zinc-400">{{ funcao }}</p>
                    <p class="text-base text-zinc-400 mb-3">{{ periodo }}</p>
                    <p>{{ descricao }}</p>
                </div>
            </div>

            <div class="mt-4 flex items-center space-x-4">
                <img v-for="tecnologia in tecnologias" class="w-8" :src="tecnologia.img" alt="">
            </div>

        </div>
    </section>
</template>

<script setup>
import { defineProps } from 'vue'
import PHP from '../../public/PHP.png'

defineProps({
    periodo: String,
    nome: String,
    funcao: String,
    descricao: String,
    tecnologias: Array
})

</script>