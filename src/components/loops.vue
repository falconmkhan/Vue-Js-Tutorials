<template>
    <h1>LOOPS IN VUE JS </h1>
 <div>

    <h3>Musa is Behind these </h3>
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
            companies: ['textile' , 'softwarehouse' , 'cybercell' , 'resturant'],
            owner_info:[
                {name:'Faiz Khan' , email:'faizkhan@gmail.com' , phone:'92 3158915290'},
                {name:'Ebad Khan' , email:'ebadkhan@gmail.com' , phone:'92 3243625664'},

            ],
        }
    }
}
</script>