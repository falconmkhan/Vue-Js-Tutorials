<template>
    <h1>Methods With Parameters</h1>

    <!-- <p>{{ s_data("faiz khan") }}</p>
    <p>{{ m_data().name }}</p>
    <p>{{ m_data().email }}</p>
    <p>{{ m_data().pass }}</p> -->
    <ReusE head="Reuse Component" :data="m_data" :name="s_data" />

</template>

<script>

import ReusE from './reuse.vue';

export default {
    name:'MethodsParam',
    components:{
        ReusE
    },
    data(){
        return{
            head:null
        }
    },
    methods: {
        s_data(user_data){
            return user_data
        },
        m_data(){
            return{
                name:this.user_data,
                email:'faiz@gmail.com',
                pass:'faiz'
            }
        }
    }
}

</script>
