<template>
    <div>
        <h2 :class="$style.title">CSS 모듈 테스트</h2>

        <div :class="$style.div">

        </div>
    </div>
</template>

<scrip>
    export default {
        name: 'StyleTest2',
        created () {
            console.log(this.$style);
        },
    }
</scrip>

<style module>
    .title {
        background-color: beige;
        color: brown;
    }
    .div {
        background-color: purple;
        width: 100px;
        height: 100px;
    }
</style>