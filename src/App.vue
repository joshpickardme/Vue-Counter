<script setup>
  import {ref} from "vue"
  let count = ref(0)
</script>

<template>
  <main>
    <div>
      <h4>The current count is...</h4>
      <h1>{{ count }}</h1>
      <button @click="count--">Decrease</button>
      <button @click="count++">Increase</button>
    </div>
  </main>
</template>

<style scoped>
main {
  background-color: aliceblue;
  width: 100vw;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
}

div {
  text-align: center;
}

h4 {
  font-size: 32px;
}

h1 {
  font-size: 64px;
  padding: 0px;
  margin: 0px;
}

button {
  font-size: 32px;
  margin: 5px;
  color: var(--vt-c-indigo);
  border-radius: 6px;
  border-color: transparent;
  font-weight: 900;
  background-color: transparent;
  transition: font-size 0.1s;
}

button:hover {
  cursor: pointer;
  font-size: 35px;
  transition: font-size 0.1s;
}

</style>