<script setup>
    import {ref} from 'vue'

    const msg = ref('我是A组件中的跳跳')
</script>

<template>
    <div>
        我是A组件 -- {{ msg }}
    </div>
</template>

<style scoped>

</style>

