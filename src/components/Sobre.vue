<template>
    <section id="sobre" class="px-8 py-12 lg:px-44 items-center headline">
        <div class="block border p-4 hover:bg-[#0e0e12] cursor-pointer border-white/10 rounded-lg">
            <h1 class="text-[#27AE60] font-bold mb-4">SOBRE MIM</h1>
            <p class=" text-white">
                Lorem ipsum dolor, sit amet consectetur adipisicing elit. Ex veniam et expedita quis quod quaerat beatae eveniet sed cupiditate! Perferendis asperiores debitis excepturi illum impedit nulla nemo. Adipisci, nobis ex?
                Lorem, ipsum dolor sit amet consectetur adipisicing elit. Blanditiis earum minima animi consectetur, ipsum velit doloribus dicta laborum explicabo quibusdam. Quis eveniet, tenetur quo numquam quasi repellat dicta dolores obcaecati!
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Incidunt expedita est officiis quia laudantium cum quam, quo animi? Velit iste ab esse quod itaque praesentium fugit quo sequi delectus dolorum.
            </p>
        </div>
    </section>
</template>

<script>
export default {
    created() {
        ScrollReveal().reveal('.headline');
    }
}

</script>