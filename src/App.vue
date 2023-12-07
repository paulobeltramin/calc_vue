<script setup>
import { reactive } from 'vue';


const estado = reactive({
    value2: "",
    value1: "",
    result: "",
    calculation: "somar",


})

// function filter
const setFilter = (event) => {
    return estado.calculation = event.target.value
}


//    input 1
const valueOne = (event) => {
    return estado.value1 = estado.result = event.target.value

}
//  input2
const valueTwo = (event) => {
    return estado.value2 = estado.result = event.target.value

}

// function calculation
const getCalcFilter = () => {
    const filtro = estado.calculation;

    switch (filtro) {
        case "somar":
            return estado.value1 + estado.value2;

        case "subtrair":
            return estado.value1 - estado.value2;

        case "multiplicar":
            return estado.value1 * estado.value2;

        case "dividir":

            return estado.value1 / estado.value2

        default:

    }


}

</script>

<template>
    <main class="container bg-secondary p-5">
        <h1 class="text-center mt-4 text-white mb-4">Calculadora</h1>

        <div class="row ">
            <form class="d-flex  flex-column align-items-center">

                <div class=" w-50 mb-4 bg-black text-center text-white p-3 fs-4">
                    {{ getCalcFilter() }}
                </div>

                <div class="col">
                    <input class="form-control w-100 mb-4" type="number" placeholder="digite o valor 1" @keyup="valueOne">
                    <input class="form-control w-100 " type="number" placeholder="digite o valor 2" @keyup="valueTwo">

                    <select class="bg-black text-white fw-bold p-1 mt-4" @change="setFilter">
                        <option value="somar">Somar</option>
                        <option value="subtrair">Subtrair</option>
                        <option value="multiplicar">Multiplicar</option>
                        <option value="dividir">Dividir</option>
                    </select>

                </div>

            </form>

        </div>
    </main>
</template>
  
<style scoped></style>




