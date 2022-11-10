<template>
    <div>
        <button @click="count++">add 1</button><br>
        <button @click="dropdown=!dropdown">drop</button>
        <div v-if="dropdown">go down</div>
        <hr>
        <div>onchange</div>
        <input type="text" @change="count++">
        <hr>
        <div>Count is : {{count}}</div>
        <hr>

        <div>v-model</div>
        <input v-model="name" type="text" class="border-2"/>
        <div>{{name}}</div>
        <font-awesome-icon icon="fa-solid fa-bomb" class="text-9xl"/>
    </div>
</template>

<script>
export default {
    data()
    {
        return {
            count: 0,
            dropdown: false,
            name: "doc"
        }
    }

}
</script>

<style>

</style>