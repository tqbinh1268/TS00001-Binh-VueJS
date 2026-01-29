<template lang="">
    <div>
        <h1 v-on:click.right="handleClick('Hello Vue!')">Slide 7</h1>
        <input type="" name="" v-model.lazy.trim="myName"> <br>
        <p>{{ myName }}</p>
    </div>
</template>
<script setup>
import { ref } from 'vue';
const myName = ref('');
const handleClick = (message) => {
    alert(myName.value);
};
</script>
<style lang="">

</style>