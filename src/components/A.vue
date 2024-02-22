<script setup>
    import {ref} from 'vue'

    const person = ref({
        name: 'wax'
    })

    const call = () => {
        window.location.href = 'tel:' + 18101930232;
    }

</script>

<template>
    <div>
        我是A组件 -- {{ person.name }}

        <button @click="call">点我打电话</button>

    </div>
</template>

<style scoped>

</style>

