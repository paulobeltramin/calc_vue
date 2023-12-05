<script setup>

</script>

<template>
    <div class="container">
        <header class="body ">
            <div>
                <h1 class="fw-bold text-center mt-4 p-3 text-white">Calculadora</h1>
            </div>
        </header>

        <section>
            <div class="container_body">
                <div class="d-flex justify-content-center  align-center p-4 bg-black w-100 ">
                    <span class="text-white fw-bold fs-2">124,00</span>
                </div>

                <div class="row mt-4">
                    <div class="col d-flex fw-bold fs-2 text-center fs-3 ">
                        <p class="col-3  border border-secundary pointer p-1 ">
                            C
                        </p>

                        <p class="col-3  border border-secundary pointer p-1">
                            ()
                        </p>

                        <p class="col-3  border border-secundary pointer p-1">
                            %
                        </p>

                        <p class="col-3 pointer">
                            ÷
                        </p>
                    </div>
                </div>

                <div class="row">
                    <div class="col d-flex fw-bold p-3 text-center fs-3 ">
                        <p class="col-3  border border-secundary pointer p-1">
                            4
                        </p>

                        <p class="col-3  border border-secundary pointer p-1">
                            5
                        </p>

                        <p class="col-3  border border-secundary pointer p-1">
                            6
                        </p>

                        <p class="col-3 pointer">
                            x
                        </p>
                    </div>
                </div>

                <div class="row">
                    <div class="col d-flex fw-bold p-3 text-center fs-3 ">
                        <p class="col-3  border border-secundary pointer p-1">
                            4
                        </p>

                        <p class="col-3  border border-secundary pointer p-1">
                            5
                        </p>

                        <p class="col-3  border border-secundary pointer p-1">
                            6
                        </p>

                        <p class="col-3 pointer fs-1">
                            -
                        </p>
                    </div>
                </div>

                <div class="row">
                    <div class="col d-flex fw-bold p-3 text-center fs-3 ">
                        <p class="col-3  border border-secundary pointer p-1">
                            1
                        </p>

                        <p class="col-3  border border-secundary pointer p-1">
                            2
                        </p>

                        <p class="col-3  border border-secundary pointer p-1">
                            3
                        </p>

                        <p class="col-3 pointer">
                            +
                        </p>
                    </div>
                </div>

                <div class="row">
                    <div class="col d-flex fw-bold p-3 text-center fs-3 ">
                        <p class="col-3  border border-secundary pointer p-1">
                            +/-
                        </p>

                        <p class="col-3   border border-secundary pointer p-1">
                            0
                        </p>

                        <p class="col-3  border border-secundary pointer p-1">
                            ,
                        </p>

                        <p class="col-3 pointer ">
                            =
                        </p>
                    </div>
                </div>
            </div>
        </section>
    </div>
</template>
  
<style scoped>
.body {
    background-color: grey;
}

.container_body {
    background-color: rgb(223, 196, 162);
    height: 600px;
    width: 400px;
    margin: 0 auto;
}

.pointer {
    cursor: pointer;

}

.pointer:hover {
    background-color: antiquewhite;
}
</style>




