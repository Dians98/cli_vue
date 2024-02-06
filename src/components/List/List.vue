<template>
    <ul class="list-group  ">
        <li v-for="(fruit,index) in fruits" v-bind:key="index" class="list-group-item lightBlue" >{{ fruit }}</li>
    </ul>
</template>

<script>
    export default 
    {
        // eslint-disable-next-line vue/multi-word-component-names
        name : 'list',
        data()
        {
            return {
                fruits : ["Pomme", "Raisin","Banane"]
            }
        }
    }
</script>

<style scoped src="./List.css">

</style>