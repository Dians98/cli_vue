
<template>
    <div>
        <h4>{{ txt }}</h4>
        <List></List>
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
                txt: "Bienvenue sur cette page en Vue.js"
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