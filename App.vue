<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <TextInput msg="Nom " />
    <TextInput msg="Prénom " /><!-- Envoyer une props à un composant -->
    <DateInput msg="date " />
    <TextAreaInput msg="description " /> 
    <SelectInput msg="profession " />
    <RadioInput msg="Sexe " />
    <CheckBoxInput msg="Compétences : " />
  </div>
</template>

<script>
import TextInput from "./components/TextInput.vue";
import DateInput from "./components/DateInpute.vue";
import TextAreaInput from "./components/TextAreaInput.vue";
import SelectInput from "./components/SelectInput.vue";
import RadioInput from "./components/RadioInput.vue";
import CheckBoxInput from "./components/CheckBoxInput.vue";


export default {
  
  name: "App",
  components: {
    TextInput,
    DateInput,
    TextAreaInput,
    SelectInput,
    RadioInput,
    CheckBoxInput,
  },
  data: function () {
    return {
    
      name: "HUHO",
      email: {
        value: "huho@gmail.com",
      },
    };
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
#textarea{
    height: 70px;
    width: 180px;
    
}

</style>
