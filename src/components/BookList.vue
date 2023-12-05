<template>
        <!-- <ul>
            <li v-for="(liItem) in bookList" >{{ liItem.title }}</li>
        </ul> -->
        <!-- <label for="nev">Név:</label>
        <input type="text" id="nev" v-model="name">
        <button @click="$emit('nameSend', name)">Elküld</button> -->
</template>

<script setup>
import {ref} from 'vue';

const name = ref("")

defineProps(["bookList"])
</script>