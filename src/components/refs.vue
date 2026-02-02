<template>
    <h1>{{ head }}</h1>
    <h4>refs is acutally get data from templete thorugh $refs, is buit in property</h4>
    <label for="id">Input: </label>
    <input type="text" id="id" ref="input">
    <p></p>
    <button v-on:click="click()">Click </button>
    <p></p>
    <div ref="box">this is box work on click</div>
    <button v-on:click="box()">Box</button>
</template>

<script>
export default {
    name:'RefS',
    props:{
        head:String,
    },
    methods:{
        click(){
            // $refs is a pre define method
            // this.$refs.input.focus();
            let val=this.$refs.input.value;
            this.$refs.input.style.background="black";
            this.$refs.input.style.color="white";
            console.warn(val)
        },
        box(){
            this.$refs.box.style.border="2px solid black";
            this.$refs.box.style.padding="30px";


        }
    }
}
</script>