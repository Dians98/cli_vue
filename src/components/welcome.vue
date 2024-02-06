<template>
    <div>
        <h4>{{ txt }}</h4>
        <!--
            On passe le props au component enfant en utilisant v-bind:nomDuPropsEnfant="dataParentAPasser"
        -->
        <List v-bind:fruitCategory="category"></List>
    </div>
</template>

<script>
import List from './List/List.vue'

    export default 
    {
        // eslint-disable-next-line vue/multi-word-component-names
        name: 'welcome',
        data()
        {
            return { 
                txt: "Bienvenue sur cette page en Vue.js",
                category:['cat1', 'cat2', 'cat 3']
            }
        },
        components:
        {
            'List' : List
        }
    }
</script>

<style scoped>

</style>