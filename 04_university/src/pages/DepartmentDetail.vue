<template>
    <div>
        <h2>학과 상세 조회</h2>
        <p>{{ currentRoute.fullPath }}</p>
        <p>{{ currentRoute.path }}</p>
        <p>{{ currentRoute.params }}</p>
        <p>{{ currentRoute.params.no }}</p>
        <p>{{ currentRoute.query }}</p>

    </div>
</template>

<script setup>
    import { useRoute } from 'vue-router';

    const currentRoute = useRoute();
</script>

<style lang="scss" scoped>

</style>