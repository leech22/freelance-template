<template>
    <div class="py-4 w-screen">
        <div class="text-center text-4xl font-sans tracking-widest text-medium text-gray-700 py-4 uppercase">
            Portfolio
        </div>
        <div class="grid grid-cols-1 md:grid-cols-3 gap-4">
            <slot name="project"></slot>
        </div>
    </div>
</template>
<script>

export default { 
}
</script>