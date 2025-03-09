<script setup>
    //引入 ref 函数
    import { ref,onMounted } from "vue";

    //声明响应式数据
    const count = ref(0);
    function increment() {
        count.value++;
    };

    //钩子函数
    onMounted(() => {
        console.log('Vue mounted')
    });

</script>

<template>
    <button @click="increment">count:{{ count  }}</button>
</template>

<style scoped>

</style>