<template>
    <div>
        <table class="table table-striped table-hover text-center">
            <thead>
                <tr>
                    <th>학과 번호</th>
                    <th>학과 이름</th>
                    <th>계열</th>
                    <th>개설 여부</th>
                    <th>정원</th>
                    <th>삭제</th>
                </tr>
            </thead>
            <tbody>
                <tr v-for="department in departments" :key="department.no">
                    <td>{{ department.no }}</td>
                    <td>{{ department.name }}</td>
                    <td>{{ department.category }}</td>
                    <td>{{ department.openYn }}</td>
                    <td>{{ department.capacity }}</td>
                    <td>
                        <button type="button" class="btn btn-outline-danger">삭제</button>
                    </td>
                </tr>
            </tbody>
        </table>
    </div>
</template>

<script setup>
    const props = defineProps({
        departments: {
            type: Array,
            required: true
        }
    });
</script>

<style scoped>

</style>