<template>
    <div class="relative cursor-pointer">
        <div>
            <div class="block overflow-hidden">
                <a :href="linkURL" target="_blank">
                <img :class="{
                    'transition':true, 
                    'duration-500':true, 
                    'ease-in-out':true, 
                    'transform':true,
                    '-translate-y-1':hover,
                    'scale-125':hover,
                    'object-cover':true,
                    }" :src="imgURL">
                    </a>
            </div>
            <div class="absolute w-full h-full top-0" @mouseover="hover=true" @mouseleave="hover=false">
                <div :class="{
                    'flex': true,
                    'h-full': true,
                    'transition':true, 
                    'duration-500':true, 
                    'ease-in-out':true, 
                    'product-hover': hover
                    }">
                    <div class="my-auto px-10" v-if="hover">
                        <div class="text-white font-bold text-3xl font-sans tracking-wide">
                            {{name}}
                        </div>
                        <div class="text-white font-light text-md font-sans">
                            {{description}}
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    data: () => {
        return {
            hover: false
        }
    },
    props: {
        imgURL: {
            type: String,
            default: "/img/product-1.jpg"
        },
        linkURL:{
            type: String,
            default: "https://github.com"
        },
        name: {
            type: String,
            default: "Project Name"
        },
        description: {
            type: String,
            default: "Short Descriptions"
        }
    }
}
</script>
<style>
.product-hover{
    background-color: rgb(0,0,0,.8)
}
</style>