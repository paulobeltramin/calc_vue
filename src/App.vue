<script setup>
import { reactive } from 'vue';
import Forms from "./components/Forms.vue";

const state = reactive({

    value2: "",

    value1: "",

    calculation: "somar",

    result: "0",

});

// function filter
const filterSelect = (event) => {
    return state.calculation = event.target.value
};


//    input 1
const oneValue = (event) => {
    return state.result = state.value1 = event.target.value


};
//  input2
const twoValue = (event) => {
    return state.result = state.value2 = event.target.value;


};

// function calculation
const setCalcFilter = () => {
    const filtro = state.calculation;

    switch (filtro) {
        case "somar":
            return Number(state.value1) + Number(state.value2);

        case "subtrair":
            return state.value1 - state.value2;

        case "multiplicar":
            return state.value1 * state.value2;

        case "dividir":
            return state.value1 / state.value2;

        default:

    };

};

</script>

<template>
    <Forms :filter="setCalcFilter()" :one-value="oneValue" :two-value="twoValue" :value1="state.value1"
        :value2="state.value2" :filter-select="filterSelect" />
</template>
  
<style scoped></style>




