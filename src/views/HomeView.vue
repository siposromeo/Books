<template>
    <input type="checkbox" @change="isListComp = !isListComp">

    <book-list v-if="isListComp" @nameSend="dataReceive" :bookList="bookList" />
    <book-table v-if="!isListComp" :bookList="bookList" />

    <div v-for="book in bookList">
        <book-card :konyv="book" v-if="isListComp"/>
    </div>
</template>

<script setup>
import { ref } from 'vue';
import books from '../bookdata'
import BookTable from '../components/booktable.vue';
import BookList from '../components/BookList.vue';
import BookCard from '../components/BookCard.vue';

let bookList = ref([])
let isListComp = ref(true);
bookList.value = books

const nev = ref("")

const dataReceive = (par) => {
    nev.value = par
}

</script>