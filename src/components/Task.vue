<template>
    <div :class="[task.completed ? 'completed' : '', 'task']">
        <h3>{{ task.title }}</h3>
        <p>{{ task.day }}</p>
        <i class="fa-solid fa-xmark"></i>
    </div>
</template>

<script>
    export default {
        name: 'TaskComponent',
        props: {
            task: Object
        }
    }
</script>

<style>

    .fa-solid {
        position: absolute;
        top: 10px;
        right: 10px;
    }

    .task {
        position: relative;
        font-size: 1rem;
        padding: .5rem;
        border: 1px solid #ccc;
        border-radius: 7px;
        margin: 1rem 0;
        background-color: #fff;
    }

    .task p {
        margin-top: -1rem;
    }

    .task.completed {
        border: 3px solid green;
    }
</style>