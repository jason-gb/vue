<template>
    <main>
        <h2>학과 등록</h2>
        <DepartmentForm submitButtonText="학과 등록" :initFormData/>
    </main>
</template>

<script setup>
    import DepartmentForm from '@/components/DepartmentForm.vue';
    import { ref } from 'vue';
</script>
    const formData = ref ({
        name:'',
        category: '',
        openYn: 'Y',
        capacity: 30
    });
<style scoped>
</style>