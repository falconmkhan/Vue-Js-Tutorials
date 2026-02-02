<template>
    <h1>{{ head }}</h1>
    <!-- <form action=""> -->

        <input type="text" v-model="form.name" placeholder="name">
        <br><br>
        <input type="text" v-model="form.code" placeholder="code">
        <br><br>
        <label for="j">JS</label>
        <input type="checkbox" id="j" v-model="form.feild" value="js">

        <label for="p">PHP</label>
        <input type="checkbox" id="p" v-model="form.feild" value="php">
        <br>
        <button type="submit" v-on:click="done()">Done</button>
    <!-- </form> -->
</template>

<script>
export default {
    name:'formValid',
    props:{
        head:String,
    },
    data(){
        return{

        form:{
            name:'',
            code:'',
            feild:[]
        },
        error:[],
      }
    },
    methods:{
        done(){
            this.error = [];
            for(let item in this.form){
                // console.warn(this.form[item])
                if(this.form[item] === '' || this.form[item].lenght === 0){
                    // console.warn(this.form,this.error)
                    this.error.push(item)
                    // console.warn(this.error.lenght)
                }
            }
            if(this.error.length === 0){
                alert(
                    'submitted'
                )
            }
            console.log(this.form,this.error)
            
        }
    }
}
</script>