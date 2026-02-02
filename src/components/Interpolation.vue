<template>
    <h1>Practices</h1>
    <h2>interpolation And Data</h2>
    <h3>{{ 10+10 }}</h3> 
    this is called interpolation
    <h3>{{ "helloworld".length }}</h3>

    <p>{{ name="faiz" }}</p>
    <!-- value can change in vue but not in angular -->
    <p>{{ email }}</p>
    <p>{{ data("{faizkhan} {nomail@test.com}") }}</p>
</template>

<script>

export default {
    name:'InterpolationData',
    data() {
        return{
            name:"faiz_khan",
            email:"faiz@gmail.com",
            data:function(data){
                return data
            }
        }
    }
}

</script>