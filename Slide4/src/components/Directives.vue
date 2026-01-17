<template lang="">
    <div>
        <input type="text" v-bind:name="fullName" v-bind:value="name">
        <h2>{{name}}</h2>
        <h3>{{ fullName }}</h3>
        <input type="" name="" value="name">
    </div>
</template>
<script>
export default {
    data(){
        return{
            name : 'Tran Quang Binh',
            fullName:''
        }
    }
}
</script>
<style lang="">
    
</style>