<script setup>
    import {ref} from 'vue'

    const msg1 = ref('我是A组件中的哈哈')

</script>

<template>
    <div>
        我是A组件 -- {{ msg1 }}
    </div>
</template>

<style scoped>

</style>

