<template>
    <section class="bg-[#171717]">
        <div class="flex flex-col items-center justify-center min-h-screen relative">
            <div class="flex border-2 border-[#202020] p-3 justify-center rounded-full">
                <img class="rounded-full w-60" :src="me" alt="">
            </div>
            <div class="text-center text-4xl text-white mt-8">
                <div class="mb-2">
                    <h1 class="font-semibold text-white">Olá! Sou</h1>
                    <h1 class="font-semibold text-white">Tony Albert</h1>
                </div>
                <p class="text-[#828282] text-base">Desenvolvedor Fullstack</p>
            </div>
            <div class="block mt-6">
                <a href=""><button class="text-white text-sm py-3 w-full px-6 font-semibold bg-[#27AE60] hover:bg-[#1A5E37] transition-colors">Download CV</button></a>
                <a href=""><button class="text-white text-sm py-3 w-full px-6 font-semibold border mt-3 hover:bg-white hover:text-[#27AE60] transition-colors">Contate-me</button></a>
            </div>
            <div class="absolute bottom-16 animate-bounce">
                <img src="/arrow.svg" alt="">
            </div>
        </div>
    </section>
</template>

<script>
import Me from '/me.png'

export default {
    data() {
        return {
            me: Me
        }
    }
}


</script>



