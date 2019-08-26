<template>
    <div class="home">
        <h1>{{ msg }}</h1>
        <label for="">Primer Numero</label><br />
        <input type="text" id="f_value"><br />
        <label for="">Segundo Numero</label><br />
        <input type="text" id="s_value"><br />
        <button v-on:click="_plus">Suma</button>

    </div>
</template>



<script>
    export default {
        name: 'home.vue',
        methods: {

            _plus: function () {

                var a = Number(document.getElementById('f_value').value);
                var b = Number(document.getElementById('s_value').value);
                var suma = a + b;
                alert("La suma de " + a + "+" + b + "es: " + suma);
            }

        }
    }

</script>
<style scoped>
</style>