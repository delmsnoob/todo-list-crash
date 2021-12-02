<template>
    <header>
        <Button @btn-click="$emit('toggle-add-task')" />
        <h1>{{ title }}</h1>
    </header>
</template>

<script>
import Button from './Button'
export default {
    name: 'Header',
    props: {
        title: String,
        showAddTask: Boolean
    },
    components: {
        Button
    }
}
</script>

<style scoped>
header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 20px;
}

h1 {
    align-items: center;
}
</style>