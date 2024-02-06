<template>
    <ul class="list-group">
        <li v-for="(fruit,index) in fruits" v-bind:key="index" class="list-group-item lightBlue" >{{ fruit }}</li>
        <p>{{ fruitCategory[0] }}</p>
        <h4>Reversed : {{ reverseCategory() }}</h4>
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
        },
        /**
         * Props comme propriété, sont les moyens utilisés pour passer des données parent->enfant
         */
        props:
        {
            fruitCategory :
            {
                type : Array,
                required : true
            }
        },

        methods:
        {
            reverseCategory()
            {
                return this.fruitCategory[0].split('').reverse().join('');
            }
        }
    }
</script>

<style scoped src="./List.css">

</style>