<template>
<div class="bg-[url(./src/assets/image/NightSky.jpg)]">
    <div class="left-0 top-0">
        <Router-link to="/" class="container mx-auto border-2 p-2 rounded-lg m-0 object-none  bg-indigo-500"> Go Home </Router-link>
    </div>
    <center>
        <h1 class="text-4xl font-serif">Our Profile</h1>
    </center>
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
    ></profileCard>
    <profileCard
        name= "Thanawat Potidech"
        nickname= "Boss"
        age= "18-year-old"
        birthday= "18-September-2003"
        study= "Kasetsart Uneversity"
        status= "KU-82 SC-57 CS-37"
    ></profileCard>
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