<script setup>
  

</script>

<template>
    <main class="container bg-secondary p-5">
        <h1 class="text-center mt-4 text-white mb-4">Calculadora</h1>

        <div class="row ">
            <form class="d-flex  flex-column align-items-center">

                <div class=" w-50 mb-4 bg-black text-center text-white p-3 fs-4">
                    1250
                </div>

                <div class="col">
                    <input class="form-control w-100 mb-4" type="number" placeholder="digite o valor 1">
                    <input class="form-control w-100 " type="number" placeholder="digite o valor 2">

                    <select class="bg-black text-white fw-bold p-1 mt-4">
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




