<template>
    <nav class="backdrop-blur-md bg-black/10 w-full py-5 px-8 lg:px-44 fixed z-20">
        <div class="flex justify-between">
            <div class="text-white">
                <h1>Logo</h1>
            </div>

            <div>
                <ul class="hidden lg:flex text-white font-semibold space-x-6 transition">
                    <li class="hover:text-[#27AE60]"><a href="">Home</a></li>
                    <li class="hover:text-[#27AE60]"><a href="#sobre">Sobre</a></li>
                    <li class="hover:text-[#27AE60]"><a href="">Tecnologias</a></li>
                    <li class="hover:text-[#27AE60]"><a href="">Carreira</a></li>
                </ul>
                <button class="lg:hidden" @click="ShowMenu = !ShowMenu">
                    <div class="space-y-2">
                        <span class="block w-3 h-0.5 bg-white"></span>
                        <span class="block w-6 h-0.5 bg-white"></span>
                    </div>
                </button>
            </div>
        </div>
        
    </nav>
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