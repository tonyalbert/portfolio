<template>
    <section>
        <div class="flex flex-col justify-center items-center min-h-screen reative">
            <div class="flex animate__animated animate__flipInX">
                
                <div class="flex border-2 border-[#202020] p-3 justify-center rounded-full">
                <img
                    @click="toggleImage"
                    class="rounded-full w-44 h-44 object-cover grayscale transform transition-transform"
                    :class="{ 'rotate-180': isFlipped }"
                    :src="currentImage"
                    alt=""
                >
                </div>
            </div>

            <div class="flex flex-col justify-center animate__fadeInLeft">
                <div class="text-center text-3xl text-white mt-8">
                    <div class="mb-2">
                        <h1 class="font-semibold text-white">Olá! Sou</h1>
                        <h1 class="font-semibold text-white">Tony Albert</h1>
                    </div>
                    <p class="text-[#828282] text-center text-lg">Desenvolvedor Fullstack</p>
                </div>
                <div class="block lg:flex mt-6">
                    <a href="/Currículo - Tony Albert.pdf" target="_blank"><button class="text-white border border-[#27AE60] hover:border-[#27AE60] text-sm xl:text-md py-3 w-full px-6 font-semibold bg-[#27AE60] hover:bg-[#1A5E37] transition-colors hover:shadow-2xl shadow-[#27AE60]">Download CV</button></a>
                    <a><button class="text-white text-sm py-3 w-full px-6 font-semibold border mt-3 lg:mt-0 xl:text-md xl:mt-0 xl:ml-6 hover:bg-white hover:text-[#27AE60] transition-colors">Contate-me</button></a>
                </div>
            </div>

            <a class="absolute bottom-12 lg:bottom-8 2xl:bottom-16 animate-bounce" href="#sobre">
                <img  :src="Arrow" alt="">
            </a>
        </div>

        
    </section>
</template>

<script>
import Me from '/me.png'
import MeDraw from '/meDraw.jpg'
import Arrow from '/arrow.svg'

export default {
    data() {
        return {
            me: Me,
            Arrow,
            isFlipped: false,
            images: [
                Me,
                MeDraw  
            ]
        }
    },
    computed: {
        currentImage() {
            return this.images[this.isFlipped ? 1 : 0];
        }
    },
    methods: {
        toggleImage() {
        this.isFlipped = !this.isFlipped;
        }
    }
}
</script>



