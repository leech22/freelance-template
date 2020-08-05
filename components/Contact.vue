<template>
    <div class="flex flex-col w-screen h-full py-10 items-center">
        <div class="text-4xl font-sans tracking-widest text-medium text-gray-700 py-4 uppercase">
            contact 
        </div>
        <div class="text-lg font-sans tracking-widest text-gray-700">
            {{email}}
        </div>
        <div class="text-lg font-sans tracking-widest text-gray-700">
            {{phone}}
        </div>
    </div>
</template>
<script>
export default {
    props: {
        email: {
            type: String,
            default: "Your Email"
        },
        phone : {
            type: String,
            default: "Your Phone"
        }
    }
}
</script>