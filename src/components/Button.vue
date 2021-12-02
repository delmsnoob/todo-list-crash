<template>
    <i @click="onClick()" class="temp fa fa-bars"></i>
</template>

<script>
export default {
    name: 'Button',
    props: {
        color: String
    },
    methods: {
        onClick() {
            this.$emit('btn-click')
        },
    }
}
</script>

<style scoped>
.temp {
    font-size: 2.2em;
    /* margin-right: 5px; */
}
</style>