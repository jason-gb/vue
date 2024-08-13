<!-- 보이는 부분 -->
<template>
  <main>
    <h2>Vue.js 기초</h2>
    <!-- <Directive1/> -->
    <!-- <Directive2/> -->
    <!-- <Options/> -->
    <!-- <Event/> -->
    <StyleTest/>
    <StyleTest2/>
  </main>
</template>

<!-- 컴포넌트에서 쓰는 기능 -->
<script>
  import Directive1 from './components/Directive1.vue';
  import Directive2 from './components/Directive2.vue';
  import Options from './components/Options.vue';
  import Event from './components/Event.vue';
  import StyleTest from './components/StyleTest.vue';
  import StyleTest2 from './components/StyleTest2.vue';

  export default {
    name: 'App',
    components: {
      Directive1, // Directive1: Directive1
      Directive2,
      Options,
      Event,
      StyleTest,
      StyleTest2
    }

  }
</script>

<!-- 컴포넌트에서 쓰는 디자인 -->
<style scoped>

</style>