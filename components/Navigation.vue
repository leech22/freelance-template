<template>
    <div class="absolute w-full top-0 z-10">
        <div class="flex justify-between px-8 pt-8 pb-4 items-center">
            <div>
                <img class="w-32" :srcset="logoURL" />
            </div>
            <ul class="md:flex">
                <li class="py-2 px-4 text-sm font-sans antialiased font-light">
                    <a class="transition-all duration-500 ease-in-out tracking-widest text-gray-700 hover:shadow-xl hover:text-white hover:no-underline hover:outline-none" href="#home">HOME</a>
                </li>
                <li class="py-2 px-4 text-sm font-sans antialiased font-light">
                    <a class="transition-all duration-500 ease-in-out tracking-widest text-gray-700 hover:shadow-xl hover:text-white hover:no-underline hover:outline-none" href="#portfolio">PORTFOLIO</a>
                </li>
                <li class="py-2 px-4 text-sm font-sans antialiased font-light">
                    <a class="transition-all duration-500 ease-in-out tracking-widest text-gray-700 hover:shadow-xl hover:text-white hover:no-underline hover:outline-none" href="#strength">STRENGTH</a>
                </li>
                <li class="py-2 px-4 text-sm font-sans antialiased font-light">
                    <a class="transition-all duration-500 ease-in-out tracking-widest text-gray-700 hover:shadow-xl hover:text-white hover:no-underline hover:outline-none" href="#contact">CONTACT</a>
                </li>
            </ul>
        </div>
    </div>
</template>
<script>

export default {
    props: {
        logoURL : {
            type: String,
            default: '/img/logo.png'
        }
    }
}
</script>
