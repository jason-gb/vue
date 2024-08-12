<!-- 보이는 부분 -->
<template>
  <main>
    <h2>App 컴포넌트 생성</h2>
    <p>{{ message }}</p>
  </main>
</template>

<!-- 컴포넌트에서 쓰는 기능 -->
<script>
  export default {
    data: function() {
      return {
        message : '안녕하세요오'
      }
    }
  }
</script>

<!-- 컴포넌트에서 쓰는 디자인 -->
<style scoped>

</style>