<template>
    <h1>IF ELSE IN VUE</h1>
    
    <h3 v-if="condition==0">IF CONDITION</h3>
    <h3 v-else-if="condition==1">IF-ELSE CONDITION</h3>
    <h3 v-else>ELSE CONDITION</h3>

    <h3 v-if="toggle">SHOW</h3>
    <h3 v-else>HIDE</h3>
    <button v-on:click="toggle=!toggle">Toggle</button>

</template>

<script>

export default {
    name: 'IfElse',
    data(){
        return{
            condition:0,
            toggle:1
        }
    }
}

</script>