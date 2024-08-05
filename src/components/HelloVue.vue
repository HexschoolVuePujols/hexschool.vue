<template>
    <div>
        num: <span>{{ num }}</span>
        <br>
        <button v-on:click="numPlusOne">按一次加 1</button>
    </div>
</template>

<script setup>
import {ref} from 'vue'
    let num = ref(1);

    function numPlusOne(){
        num.value++
    }
</script>

<style scoped></style>