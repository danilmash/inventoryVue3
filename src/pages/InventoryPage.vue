<template>
    <div class="page inventory-page">
        <div class="wrapper inventory-page__wrapper">
            <div class="inventory-page__grid">
                <Card class="inventory-page__profile"></Card>
                <div style="background-color: #4d4d4d; aspect-ratio: 1"></div>
            </div>
            <Card class="inventory-page__footer-card"></Card>
        </div>
    </div>
</template>

<script setup>
import Card from "@/components/Card.vue";
</script>

<style lang="scss" scoped>
.inventory-page {
    &__wrapper {
        max-width: 900px;
    }

    &__grid {
        height: fit-content;
        display: grid;
        gap: 12px;
        grid-template-columns: 250px minmax(500px, 800px);
    }

    &__footer-card {
        margin-top: 24px;
    }
}
</style>
