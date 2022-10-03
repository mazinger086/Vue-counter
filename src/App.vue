<script>

export default {
  data: () => ({
    contador: 100
  }),
  methods: {
    substract(){
      this.contador -= 1
    },
    add(){
      this.contador += 1
    },
    reset() {
      this.contador = 10
    }
  }  
}

</script>

<template>
  <img src="./assets/logo.svg" alt="logo vue" width="125" height="125" />
  <small>
    <h1>Hola mundo desde Vue.js 3</h1>
  </small>

  <h2>Contador: {{contador}}</h2>

  <div class="buttons">
    <button @click="add">+1</button>
    <button @click="substract">-1</button>
    <button @click="reset">Reset</button>
  </div>
  
</template>

<style scoped>

h1 {
  font-weight: bolder;
  font-family: 'Manrope', sans-serif;
}

h2 {
  font-size: 2.5rem;
}

small {
  color: #777;
}

.buttons {
  display: flex;
  gap: 5px;
}

.buttons button {
  cursor: pointer;
  font-size: 1rem;
  padding: .5rem;
}
</style>
