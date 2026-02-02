<template>
    <!-- <InterpolationData  /> -->
    <!-- <MethodsParam/> -->
    <!-- <EventS /> -->
    <!-- <TwoWay /> -->
    <!-- <FetchData /> -->
    <!-- <IfElse /> -->
     <!-- <LoopS /> -->
      <!-- <ParenrElem /> -->
      <!-- <ChildElem /> -->
    <!-- <HtmlBind head="Html Binding"/> -->
     <!-- <RefS head="Refs In Vue Js" /> -->
      <!-- <formS head="Get Form Data" /> -->
       <formValid head="Form Validation" />
</template>

<script>

// import InterpolationData from './components/Interpolation.vue'
// import MethodsParam from './components/methods_params.vue';
// import EventS from './components/events.vue';
// import TwoWay from './components/binding.vue';
// import FetchData from './components/fetch.vue';
// import IfElse from './components/if_else.vue';
// import LoopS from './components/loops.vue';
// import ParenrElem from './components/parent.vue';
// import ChildElem from './components/child.vue';
// import HtmlBind from './components/html_binding.vue';
// import RefS from './components/refs.vue';
// import formS from './components/forms.vue';
import formValid from './components/form_validation.vue';


export default {
    name: 'MyAppComponent',
    head:null,
    components: {
        // InterpolationData,
        // MethodsParam,
        // EventS,
        // TwoWay,
        // FetchData,
        // IfElse,
        // LoopS,
        // ParenrElem,
        // ChildElem,
        // HtmlBind,
        // RefS,
        // formS,
        formValid,
    }
};

</script>


<!-- scoped -->
<style>
#myapp {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
}
</style>