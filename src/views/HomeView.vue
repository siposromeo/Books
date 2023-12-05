<template>
    <!-- <button @click="isListComp = !isListComp">
        <span v-if="isListComp">Table</span>
        <span v-else>List</span>
    </button> -->
    <br>
    <span>Megjelenités táblázatban: </span><input type="checkbox" @change="isListComp = !isListComp">

    <book-list v-if="isListComp" :bookList="bookList" />
    <book-table v-if="!isListComp" :bookList="bookList" />
</template>

<script setup>
import { ref } from 'vue';
import books from '../bookdata'
import BookTable from '../components/BookTable.vue';
import BookList from '../components/BookList.vue';


let bookList = ref([])
let isListComp = ref(true);
bookList.value = books



</script>