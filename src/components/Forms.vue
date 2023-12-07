
<script setup>

const props = defineProps([

    "value1",
    "value2",
    "filter",
    "oneValue",
    "twoValue",
    "filterSelect"
])


</script>



<template>
    <main class="container bg-secondary p-5 rounded-5 mt-5 ">
        <h1 class="text-center mt-4 text-white mb-4">Calculadora</h1>

        <div class="row ">
            <form class="d-flex  flex-column align-items-center">

                <input type="url" class=" w-50 mb-4 bg-black text-center text-white p-3 fs-4 rounded-4"
                    :value="props.filter" />

                <div class="col">
                    <input :value="props.value1" class="form-control w-100 mb-4" type="number"
                        placeholder="digite o valor 1" @keyup="props.oneValue">
                    <input :value="props.value2" class="form-control w-100 " type="number" placeholder="digite o valor 2"
                        @keyup="props.twoValue">

                    <select class="bg-black text-white fw-bold p-1 mt-4" @change="props.filterSelect">
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