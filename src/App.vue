<script setup>
    const nome = 'Sara'
    const idade = 15

    function inverter(texto) {
        return texto.split('').reverse().join('')
    }

    function saudacao() {
        return `Olá, ${nome}!`
    }
</script>

<template>
    <div class="info">
        <h1>Cadastro Pessoal</h1>
        <p>Nome: {{ nome }} </p>
        <p>Idade: {{ idade }}  anos</p>
        <hr />
        <p>Para completar 50 anos faltam: {{ 50 - idade }}  anos</p>
        <p>O nome tem {{ nome.length }}  caracteres</p>
        <p>O nome invertido é: {{ inverter(nome) }} </p>
        <hr />
        
        <p> {{ saudacao() }}  </p>
    </div>
</template>

<style scoped>
.info {
  background-color: rgb(24, 74, 97);
  padding: 20px 30px;
  color: rgb(255, 255, 255);
  border-radius: 10px;
}

h1 {
  color: white;
  font-weight: bold;
  font-size: 1.5em;
}
</style>
