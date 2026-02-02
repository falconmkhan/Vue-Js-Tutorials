<template>
    <h1>Parent Components</h1>
    <h2>Child name is : {{ username }}</h2>

    <!-- <form @submit.prevent="userdata">
        <input type="text" v-model="name" placeholder="name"><br><br>
        <input type="text" v-model="email" placeholder="email"><br><br>
        
        <div>
            <label for="a1">Org</label>
            <input id="a1" type="checkbox" value="org" v-model="orgs">
            <label for="a2">Software House</label>
            <input id="a2" type="checkbox" value="software" v-model="orgs" >
        </div><br>

        <button type="submit">SUBMIT</button>
    </form>
<hr><hr> -->
    <!-- <ChildElem head="CHILD VUE" 
    :name="name" :email="email" :org="orgs" :submited="submit" /> -->
<hr>

<ChildElem :childname="childname" />
</template>

<script>
import ChildElem from './child.vue'; 

export default {
    name:'ParenrElem',
    components:{
        ChildElem
    },
    data(){
        return{
            // name:null,
            // email:null,
            // orgs:[],
            // submit: false
            username:null
        }
    },
    methods:{
        // userdata(){
        //     this.submit = true
            
        // }
        childname(name){
            this.username = name
        }
    }
}

</script>