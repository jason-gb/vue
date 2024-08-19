<template>
  <div>
    <h2>Composition API</h2>
    <h3>1. 반응성을 가진 상태 데이터</h3>
    <!-- <Calc1/> -->
     <Calc2/>
  </div>
</template>

<script>
import Calc1 from './components/Calc1.vue';
import Calc2 from './components/Calc2.vue';
export default {
  setup () {

    return {}
  },
  components:{
    Calc1,
    Calc2
  }
}
</script>

<style lang="scss" scoped>

</style>