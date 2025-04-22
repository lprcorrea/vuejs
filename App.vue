<template>
  <div class="contador">
    <h1>Contador Vue</h1>
    <p>{{ contador }}</p>
    <div class="botoes">
      <button @click="contador++">+</button>
      <button @click="contador--">-</button>
      <button @click="resetar">Resetar</button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      contador: 0
    };
  },
  methods: {
    resetar() {
      this.contador = 0;
    }
  }
};
</script>

<style scoped>
.contador {
  text-align: center;
  font-family: Arial, sans-serif;
}
.botoes button {
  margin: 5px;
  padding: 10px;
  font-size: 16px;
}
</style>