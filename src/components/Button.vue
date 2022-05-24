<template>
    <button :style="{background: color}">{{ text }}</button>
</template>

<script>
    export default {
        name: 'TaskButton',
        props: {
            text: String,
            color: String,
        }
    }
</script>

<style scoped>
    button {
        font-size: 1rem;
        font-weight: bold;
        text-align: center;
        color: #ffff;
        border: none;
        border-radius: 3px;
        padding: 20px;
        margin: 10px;
        transition: all .2s ease-in-out;
    }

    button:hover {
        cursor: pointer;
        color:rgb(214, 205, 205)
    }

</style>