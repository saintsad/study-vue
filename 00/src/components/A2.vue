<template>
    <a :href="url">
        <slot></slot>
    </a>
</template>

<script>
    export default {
        name: 'A2',
        props : {
            url: String
        },
    }
</script>

<style scoped>

</style>