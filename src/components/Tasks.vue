<template>
    <div class="taskList" v-for="task in tasks" :key="task.id">
        <TaskComponent :task="task" />
    </div>
</template>

<script>
    import TaskComponent from './Task'

    export default {
        name: 'TasksList',
        props: {
            tasks: Array,
        },
        components: {
            TaskComponent,
        },
    }
</script>

<style>

</style>