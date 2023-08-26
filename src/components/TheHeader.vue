<template>

    <nav class="backdrop-blur-md w-screen bg-slate-900/10 py-5 px-8 lg:py-7 lg:px-44 fixed z-20">
        <div class="flex justify-between items-center">
            <div class="text-white">
                <a @click="ShowMenu = !ShowMenu" class="text-[#27AE60] font-bold text-3xl">{{ '<T/>' }}</a>
            </div>

            <div>
                <ul class="hidden lg:flex text-white font-semibold space-x-6 transition">
                    <li class="hover:text-[#27AE60]"><a href="#home">Home</a></li>
                    <li class="hover:text-[#27AE60]"><a href="#sobre">Sobre</a></li>
                    <li class="hover:text-[#27AE60]"><a href="#tecnologias">Tecnologias</a></li>
                    <li class="hover:text-[#27AE60]"><a href="#projetos">Projetos</a></li>
                    <li class="hover:text-[#27AE60]"><a href="">Carreira</a></li>
                </ul>
                <button class="lg:hidden" @click="ShowMenu = !ShowMenu">
                    <div class="space-y-2 z-40">
                        <span class="block w-3 h-0.5 bg-[#27AE60]"></span>
                        <span class="block w-6 h-0.5 bg-[#27AE60]"></span>
                    </div>
                </button>
            </div>
        </div>
    </nav>

    <div 
        :class="{ 'w-8/12': ShowMenu, 'w-0': !ShowMenu }" 
        class="lg:hidden fixed right-0 h-screen z-30 backdrop-blur-md bg-black/60 transition-all">

        <ul class="text-white space-y-8 text-lg font-semibold absolute top-52 left-20">
            <li @click="ShowMenu = !ShowMenu" class="hover:text-[#27AE60]"><a href="#home">Home</a></li>
            <li @click="ShowMenu = !ShowMenu" class="hover:text-[#27AE60]"><a href="#sobre">Sobre</a></li>
            <li @click="ShowMenu = !ShowMenu" class="hover:text-[#27AE60]"><a href="#tecnologias">Tecnologias</a></li>
            <li @click="ShowMenu = !ShowMenu" class="hover:text-[#27AE60]"><a href="#projetos">Projetos</a></li>
            <li @click="ShowMenu = !ShowMenu" class="hover:text-[#27AE60]"><a href="">Carreira</a></li>
        </ul>

    </div>

    
</template>

<script>
import Menu from '/Menu.svg'

export default {
    data() {
        return {
            Menu,
            ShowMenu: false
        }
    }
}
</script>