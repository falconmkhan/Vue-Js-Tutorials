<template>
    <h2>CHILD COMPONENT</h2>
    <!-- {{ name }} <br> -->
    <button v-on:click="childname(name)">Click Me</button>

    <!-- <div v-if="submited">
        {{ name }} <br>
        {{ email }} <br>
        <h3>{{ empire }}</h3> <br>
    </div>
     -->
    <!-- <ol>
        <li v-for="items in arrays" :key="items">{{ items }}</li>
        <li>{{ arrays[2] }}</li>
    </ol>
     -->

</template>

<script>

export default {
    name:'ChildElem',
    props:{
        // head:String,
        // name:String,
        // email:String,
        // empire:Array,
        // submited:Boolean,
        childname:Function
    },

    data(){
        return{
            name:'faizkhan'
        }
    },

}

</script>