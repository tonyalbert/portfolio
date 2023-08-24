<template>
    <div @click="active = !active" :class="{ 'bg-white': active }" :style="{ 'border-bottom': bdColor }" class="bg-[#212121] z-10 rounded-md group flex flex-col p-4 items-center justify-center border-b-4 border-[#0385D2] hover:bg-white transition cursor-pointer">
        <img :class="{ 'grayscale-0': active }" class="h-12 object-cover filter grayscale group-hover:grayscale-0 transition" :src="img" alt="">
        <h3 :class="{ 'text-black   ': active }" class="text-center text-white mt-4 font-semibold group-hover:text-black">{{ tecnologia }}</h3>
    </div>
</template>

<script>    
import Typescript from '/Typescript.png';

export default {
    name: 'App',
    data()  {
        return {
            Typescript,
            active: false,
        }
    },
    props: {
        img: String,
        tecnologia: String,
        bdColor: String
    }
}
</script>