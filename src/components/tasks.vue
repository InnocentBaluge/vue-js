<template>
    <div :key="task.id" v-for="task in tasks">

        <Task />
    </div>

</template>

<script>
import Task from './Task.vue'
    export default{
        name:'Tasks',
        props:{
            tasks:Array,
        },
        components:{
            Task,
        },
    }
</script>