<template>
    <h1>Two Way Binding</h1>
    <input type="text" name="" v-model="name">
    <h3> {{ name }}<hr></h3>
</template>

<script>

export default {
    name:"TwoWay",
    data(){
        return{
            name:null
        }
    }
}

</script>