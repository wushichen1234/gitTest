<script setup>
    import {ref} from 'vue'

    const person = ref({
        name: 'wax'
    })

</script>

<template>
    <div>
        我是A组件 -- {{ person.name }}
    </div>
</template>

<style scoped>

</style>

