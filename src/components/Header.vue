<template>
    <header>
        <h1>{{ title }}</h1>
        <TaskButton @click="onClick()" text="+ Add Task" color="green" />
    </header>
</template>

<script>

  import TaskButton from './Button'

export default {
    name: 'HeaderTitle',
    props: ['title'],
    components: {
        TaskButton,
    },

    methods: {
        onClick() {
           console.log('click')
        }
    }
}
</script>

<style scoped>
header {
    font-weight: bold;
    text-align: center;
    color: #2c3e50;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

h1 {
    font-size: 3rem;    
}
</style>