<template>
    <nav class="backdrop-blur-md bg-black/10 w-full py-5 px-8 fixed">
        <div class="flex justify-between">
            <div class="text-white">
                <h1>Logo</h1>
            </div>

            <div>
                <button @click="ShowMenu = !ShowMenu">
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