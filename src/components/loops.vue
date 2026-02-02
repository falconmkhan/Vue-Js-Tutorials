<template>
    <h1>LOOPS IN VUE JS </h1>
 <div>
    
    <ol>
        <li v-for="items in companies" :key="items">{{ items}}</li>
    </ol>
    for print according to index number
    <h4 v-for="items in companies" :key="items">{{ companies[1] }}</h4>
    {{ companies[0] }}
 </div> 

<div>
    <h2>OWNER INFO</h2>
    <ol>
        <li v-for="info in owner_info" :key="info">
            {{ info.name }} <br>
            {{ info.email }} <br>
            {{ info.phone }} <br><br>
        </li>
    </ol>
</div>

</template>

<script>
export default {
    name:'LoopS',
    data(){
        return{
            companies: ['designing' , 'development' , 'security'],
            owner_info:[
                {name:'Faiz Khan' , email:'faizkhan@gmail.com' , phone:'029848928428'},
                {name:'NO Name ' , email:'noname@gmail.com' , phone:'0279472497424'},

            ],
        }
    }
}
</script>