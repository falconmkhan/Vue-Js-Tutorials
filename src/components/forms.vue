<template>
    <h1>{{ head }}</h1>
    <div>
        <h2>DATA</h2>
        {{ form }}
    </div>

    <form>

        <input type="text" placeholder="Name" v-model="form.name"><br><br>
        <input type="text" placeholder="Email" v-model="form.email"><br><br>

        <div>
            <label for="js">JS: </label>
            <input type="checkbox" id="js" value="js" v-model="form.feild">

            <label for="p">PHP: </label>
            <input type="checkbox" id="p" value="php" v-model="form.feild">
        </div><br>

        <div>
            <label>Gender: </label>
            <label for="m">Male</label>
            <input type="radio" id="m" name="gender" value="male" v-model="form.gender">

            <label for="f">FeMale</label>
            <input type="radio" id="f" name="gender" value="female" v-model="form.gender">
        </div><br>

        <select v-model="form.code">
            <option value="Select Code">Select Code</option>
            <option>!#RIW9329</option>
            <option>{&9DOXp()}</option>
            <option>$*#9FIOWC</option>
        </select><br><br>

        <button v-on:click="data()">Submit</button>
    </form>
    
</template>

<script>

export default {
    name:'formS',
    props:{
        head:String,
    },

    data(){
        return{
            form:{
                name:'',
                email:'',
                feild:[],
                gender:'',
                code:''
            }
        }
    },
    methods:{
        data(){
            alert(
                `
                name is: ${this.form.name}
                email is: ${this.form.email}
                feild is: ${this.form.feild}
                gender is: ${this.form.feild}
                code is: ${this.form.code}

                `
            )
        }
    }


}
</script>