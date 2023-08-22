<template>
    <section class="bg-[#09090B]">
        <div class="flex flex-col justify-center items-center min-h-screen reative">

            <div class="flex">
                <div class="flex border-2 border-[#202020] p-3 justify-center rounded-full">
                    <img @click="runAnimation" class="rounded-full w-60" :src="me" alt="">
                </div>
            </div>

            <div>
                <div class="text-center text-4xl text-white mt-8">
                    <div class="mb-2">
                        <h1 class="font-semibold text-white">Olá! Sou</h1>
                        <h1 class="font-semibold text-white">Tony Albert</h1>
                    </div>
                    <p class="text-[#828282] text-xl">Desenvolvedor Fullstack</p>
                </div>
                <div class="block mt-6">
                    <a href="/Currículo - Tony Albert.pdf" target="_blank"><button class="text-white text-sm xl:text-xl py-3 w-full px-6 font-semibold bg-[#27AE60] hover:bg-[#1A5E37] transition-colors hover:shadow-2xl shadow-[#27AE60]">Download CV</button></a>
                    <a><button class="text-white text-sm py-3 w-full px-6 font-semibold border mt-3 xl:text-xl xl:mt-0 xl:ml-6 hover:bg-white hover:text-[#27AE60] transition-colors">Contate-me</button></a>
                </div>
            </div>

        </div>
    </section>
</template>

<script>
import Me from '/me.png'
import Arror from '/arrow.svg'

export default {
    data() {
        return {
            me: Me
        }
    },
}
</script>



