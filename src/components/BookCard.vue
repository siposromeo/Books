<template>
    <div class="row g-0">
        <div class="card mb-3">
            <div class="card-body" style="display:grid; text-align: center;">
                <h5 class="card-title">{{ konyv.title }}</h5>
                <h6 class="card-subtitle mb-2 text-body-secondary">{{ konyv.author }}</h6>
                <p class="card-text">{{ konyv.description }}</p>
            </div>
        </div>
    </div>
</template>

<script setup>
defineProps(["konyv"])
</script>