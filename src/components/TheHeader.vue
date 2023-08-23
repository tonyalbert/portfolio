<template>
    <nav class="backdrop-blur-md bg-black/10 w-full py-5 px-8 fixed">
        <div class="flex justify-between">
            <div class="text-white">
                <h1>Logo</h1>
            </div>

            <button><img :src="Menu" alt=""></button>
        </div>
    </nav>
</template>

<script>
import Menu from '/Menu.svg'

export default {
    data() {
        return {
            Menu
        }
    }
}
</script>