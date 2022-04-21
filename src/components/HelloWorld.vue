<script setup>
defineProps({
    msg: String,
    count: Number,
});
</script>

<template>
    <button @click="$emit(count++)">Tester</button>
</template>

<style scoped>
a {
    color: #42b983;
}
/* test */
</style>
