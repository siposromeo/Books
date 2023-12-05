<template>
    <ul>
        <li v-for="(liItem) in bookList" >{{ liItem.title }}</li>
    </ul>
</template>

<script setup>
    defineProps(["bookList"])
</script>