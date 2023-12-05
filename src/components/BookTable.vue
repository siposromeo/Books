<template>

    <table>
        <thead>
        </thead>
        <tbody>
            <tr v-for="book in bookList">
                <td>{{ book.title }}</td>
                <td>{{ book.author }}</td>
                <td>{{ book.author }}</td>
                <td>{{ book.description }}</td>
            </tr>
        </tbody>
    </table>

</template>

<script setup>
    defineProps(["bookList"])
</script>