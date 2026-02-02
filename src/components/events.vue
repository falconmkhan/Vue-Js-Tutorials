<template>
    <h1>EVENTS IN VUE JS</h1>
    <ol>
        <li>CLICK EVENT</li>
        <li>DOUBLE CLICK EVENT</li>
        <li>MOUSE HOVER EVENT</li>
    </ol>
    <button v-on:click="Click()">Click Me</button><br><br>
    <button v-on:dblclick="Db()">Double Click Me</button><br><br>
    <button v-on:mousemove="Mouse()">Hover Me</button>
    <h4>{{ count }}</h4>
</template>

<script>
export default {
    name:"EventS",
    data(){
        return{
            count:0
        }
    },
    methods: {
        Click(){
            // alert("clicked")
               this.count=this.count+2
        },
        Db(){
            alert("double cliked")
        },
        Mouse(){
            // alert("hover succesfullly")
            // console.warn("successfully")
        }
    }
}

</script>