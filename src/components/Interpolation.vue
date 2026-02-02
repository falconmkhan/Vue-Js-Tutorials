<template>
    <h1>Practices</h1>
    <!-- <p>
    wikipedia <br><br>
    <a href="https://en.wikipedia.org/wiki/Abu_Ubaida_(Hamas)" target="_blank">Al Hamas </a>
    </p> -->

    <h2>interpolation And Data</h2>
    <h3>{{ 10+10 }}</h3> 
    this is called interpolation
    <h3>{{ "helloworld".length }}</h3>

    <p>{{ name="musa" }}</p>
    <!-- value can change in vue but not in angular -->
    <p>{{ email }}</p>
    <p>{{ data("{mustajabkhan} {mustajabkhan2gmail.com}") }}</p>
</template>

<script>

export default {
    name:'InterpolationData',
    data() {
        return{
            name:"mustajab_khan",
            email:"mustajab@gmail.com",
            data:function(data){
                return data
            }
        }
    }
}

</script>