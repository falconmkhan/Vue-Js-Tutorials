<template>
    <h1>{{ head }}</h1>
    <!-- {{ name('faizkhan') }} <br>
    {{ name('faiz') }} <br>
    {{ name('musakazmi') }} <br>
     -->
<!-- 
    {{ data().email }} <br>
    {{ data().pass }} -->
</template>


<script>

export default {
    name:'ReusE',
    props:{
        head:String,
        name:Function,
        data:Function
    }
}

</script>