<template lang="">
    <div class="container">
        <h1 @click.right="handleClick">Slide 7</h1>
        <input type="" name="" v-model="myName" placeholder="Nhập tên" v-on:keyup.enter.shift="handleClick">
    </div>
</template>
<script setup>
import { ref } from 'vue'
    const myName = ref('')
    const handleClick = () => {
alert(myName.value);
};
</script>
<style lang="">
    
</style>