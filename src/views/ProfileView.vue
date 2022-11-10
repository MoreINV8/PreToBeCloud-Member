<template>
    <div>
        <div class="flex justify-between bg-gradient-to-l from-indigo-500">
            <div class="text-2xl font-serif p-2 m-4 font-extrabold text-sky-300">Our Profile
                <font-awesome-icon icon="fa-solid fa-cloud-moon" />
            </div>
            <Router-link to="/" class="container w-20 h-10 drop-shadow-xl p-2 m-4 rounded-lg text-violet-300  bg-indigo-500 transition duration-300 ease-in-out hover:bg-sky-300 hover:text-indigo-600 hover:scale-110 text-center font-semibold">Home </Router-link>
        </div>
        <div>
            <profileCard
                name= "Chaiyapat Sriamphai"
                nickname= "Bank"
                age= "18-year-old"
                birthday= "16-December-2003"
                study= "Kasetsart Uneversity"
                status= "KU-82 SC-57 CS-37"
                image= "/assets/image/bank.png"
            ></profileCard>
            <profileCard
                name= "Khanisorn Srisawat"
                nickname= "Tom"
                age= "18-year-old"
                birthday= "18-Febuary-2004"
                study= "Kasetsart Uneversity"
                status= "KU-82 SC-57 CS-37"
                image= "/assets/image/tom.png"
            ></profileCard>
            <profileCard
                name= "Thanawat Potidech"
                nickname= "Boss"
                age= "18-year-old"
                birthday= "18-September-2003"
                study= "Kasetsart Uneversity"
                status= "KU-82 SC-57 CS-37"
                image= "/assets/image/boss.jpg"
            ></profileCard>
        </div>
    </div>
</template>

<script>
import profileCard from "../components/icons/Profile.vue"
export default {
    data() {
        return{
            name: "Chaiyapat Sriamphai",
            nickname: "Bank",
            age: "19-year-old",
            birthday: "16-December-2003",
            study: "Kasetsart Uneversity",
            status: "KU-82 SC-57 CS-37",
        };
    },
    components:{
        profileCard,
    },
};

// <RouterLink to="ใช้ path หรือ name" แต่ง css> ชื่อปุ่ม </RouterLink>
</script>