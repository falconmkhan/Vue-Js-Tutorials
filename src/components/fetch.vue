<template>
    <h1>FETCH INPUT VALUES</h1>

    <form action="./fetch.vue"> 
        <div>
            <label for="name">Name: </label>
            <input type="text" id="name" v-model="name">
        </div><br>
        <div>
            <label for="c">Code: </label>
            <input type="text" id="c" v-model="code">
        </div><br>
        <div>
            <label for="">Company: </label>
            <label for="c1">Hacking</label>
            <input type="checkbox" id="c1" value="hack" v-model="cname">
            <label for="c2">Development</label>
            <input type="checkbox" id="c2" value="dev" v-model="cname">
        </div><br>
        <div>
            <label for="">Teacher: </label>
            <label for="s1">Mustajab</label>
            <input type="radio" id="s1" v-model="tname" value="musa" name="teacher">
            <label for="s2">Ghazali</label>
            <input type="radio" id="s2" v-model="tname" value="ghazali" name="teacher">
        </div><br>
        <input type="submit" v-on:click="getdata()">
    </form>
</template>
<script>

export default {
    name:"FetchData",
    data(){
        return{
            name:null,
            code:null,
            cname:[],
            tname:null
        }
    },
    methods: {
        getdata(){
            alert(
            `   KINDLY MAKE A PRINT OF IT
                Name: ${this.name}
                Code: ${this.code}
                Course: ${this.cname}
                Teacher: ${this.tname}`
            )
        },
        
    }
}

</script>