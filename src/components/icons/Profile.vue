<template>
    <div class="container mx-auto bg-violet-300 border-2 border-indigo-600 text-sky-300 p-4 m-3 rounded-2xl from-slate-500 bg-opacity-40 duration-500 ease-in-out hover:bg-opacity-100 hover:text-indigo-600 hover:scale-105">
        <table class="border-2 border-dashed table-auto font-mono">
            <tbody class="m-4">
                <td colspan="4" class="w-1/4">
                    <div class="border-solid border-2 border-indigo-600 m-2 rounded-full overflow-hidden">
                        <div class="h-40 w-40 bg-contain bg-no-repeat bg-center" :style="getImage(image)"></div>
                    </div>
                </td>
                <td>
                    <tr class="text-2xl font-bold">Name</tr>
                    <tr class="text-2xl  font-bold">Nickname</tr>
                    <tr class="text-2xl  font-bold">Birthday</tr>
                    <tr class="text-2xl  font-bold">Status</tr>
                </td>
                <td>
                    <tr class="text-2xl font-light">{{name}}</tr>
                    <tr class="text-2xl font-light">{{nickname}}</tr>
                    <tr class="text-2xl font-light">{{birthday}}</tr>
                    <tr class="text-2xl font-light">{{status}}</tr>
                </td>
            </tbody>
        </table>
    </div>
</template>

<script>
export default {
    props:{
        name:{
            type: String,
            default: "A B",
        },
        nickname:{
            type: String,
            default: "X",
        },
        age:{
            type: String,
            default: "0-year-old",
        },
        birthday:{
            type: String,
            default: "01-January-2000",
        },
        study:{
            type: String,
            default: "University",
        },
        status:{
            type: String,
            default: "-",
        },
        image:{
            type: String,
            default: "/assets/image/clouds.jpg"
        },
    },
    methods:{
        getImage(imagePath) {
            return {'background-image': 'url("./src/' + imagePath +'")' };
        },
    }
}
// class="w-3/4 border-solid rounded-full border-2 border-teal-600 m-2"
</script>