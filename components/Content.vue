
<template>
    <div class="relative">
        <div class="absolute top-0 w-screen h-screen bg-black bg-opacity-25 pt-32">
            <div class="flex h-full">
                <div class="flex flex-col my-auto px-5 md:px-24 lg:px-36 xl:px-64 transition-all duration-500 ease-linear">
                    <div class="font-sans font-light text-6xl mb-2 text-white md:text-8xl transition-all duration-500 ease-in-out">Hi,</div>
                    <div class="font-sans font-bold text-6xl text-white mb-2 sub-topic md:text-8xl transition-all duration-500 ease-in-out">{{name}}</div>
                    <div class="w-20 bg-white separator-line md:bg-black transition-all duration-500 ease-in-out"></div>
                    <div class="font-sans font-thin text-2xl text-white description transition-all duration-500 ease-in-out">{{job}}</div>
                </div>
            </div>
        </div>
        <div class="w-screen h-screen">
            <img :src="imgURL" class="w-full h-full object-cover"/>
        </div>
    </div>
</template>
<script>
export default {
    props:{
        imgURL: {
            type: String,
            default: '/img/bg_1.jpg'
        },
        name : {
            type: String,
            default: 'Your Name'
        },
        job : {
            type: String,
            default: 'Your Occupation'
        }
    },
}
</script>