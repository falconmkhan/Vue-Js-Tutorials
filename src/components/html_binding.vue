<template>
    <h1>{{ head }}</h1>
    <div v-html="tag"></div>

    <div v-html="btn" id="btnn"></div>

</template>


<script>

export default {
    name:'HtmlBind',
    props:{
        head:String
    },

    data(){
        return{
            tag:null,
            btn:'<button v-on:click="show()" class="btn">click me</button>'
        }
    },
    methods:{
        show(){
            this.tag = '<h2>Html Binding2</h2>'
        }
    }

}


</script>