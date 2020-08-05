<template>
    <div class="h-full w-screen">
        <div class="text-center text-4xl font-sans tracking-widest text-medium text-gray-700 py-4 uppercase">
            About
        </div>
        <div class="flex flex-col">
            <div class="w-screen">
                <div class="grid grid-cols-1 lg:grid-cols-2">
                    <div class="flex">
                        <div class="m-auto p-4">
                            <div class="font-sans font-light text-5xl text-gray-700 tracking-widest">{{profileHeader1}}</div> 
                            <div class="font-sans font-bold text-5xl text-gray-700" style="margin-top:-20px;">{{profileHeader1_2}}</div>
                            <div class="w-12 bg-gray-700 separator-line" style="margin-top:1px !important"></div>
                            <div class="mt-5 w-4/5">
                                <p class="font-serif font-hairline text-gray-500 text-sm">
                                    {{profileDescription1}}
                                </p>
                            </div>
                        </div> 
                    </div>
                    <div >
                        <img :srcset="profileImgURL_1"/>
                    </div>
                </div>
            </div>
                
            <div class="w-screen">
                <div class="grid grid-cols-1 lg:grid-cols-2">
                    <div >
                        <img :srcset="profileImgURL_2"/>
                    </div>
                    <div class="flex">
                        <div class="m-auto">
                            <div class="font-sans font-light text-5xl text-gray-700 tracking-widest">{{profileHeader2}}</div> 
                            <div class="font-sans font-bold text-5xl text-gray-700" style="margin-top:-20px;">{{profileHeader2_2}}</div>
                            <div class="w-12 bg-gray-700 separator-line" style="margin-top:1px !important"></div>
                            <div class="mt-5 w-4/5">
                            <p class="font-serif font-hairline text-gray-500 text-sm">
                                {{profileDescription2}}
                            </p>
                        </div>
                    </div> 
                </div>
            </div>
    </div>
        </div>
    </div>
</template>
<script>
export default {
    props :{
        profileImgURL_1:{
            type: String,
            default:'/img/grid_1.jpg'
        },
        profileHeader1 :{
            type:String,
            default: "Header 1"
        },
        profileHeader1_2 : {
            type: String,
            default: "Header 1-2"
        },
        profileDescription1 : {
            type:String,
            default: "Lorem ipsum dolor sit amet consectetur, adipisicing elit. Fugit quis, animi explicabo doloribus odit distinctio. Error possimus porro natus magni quod debitis dignissimos, id quia? Enim accusamus fugiat numquam consectetur."
        },

        profileImgURL_2:{
            type: String,
            default:'/img/grid_2.jpg'
        },
        profileHeader2 :{
            type:String,
            default: "Header 1"
        },
        profileHeader2_2 : {
            type: String,
            default: "Header 1-2"
        },
        profileDescription2 : {
            type:String,
            default: "Lorem ipsum dolor sit amet consectetur, adipisicing elit. Fugit quis, animi explicabo doloribus odit distinctio. Error possimus porro natus magni quod debitis dignissimos, id quia? Enim accusamus fugiat numquam consectetur."
        }
    }
}
</script>