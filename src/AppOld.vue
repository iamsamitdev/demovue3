<script setup lang="ts">
  import { ref, reactive } from 'vue' // นำเข้า ref จาก vue
  // สร้างตัวแปร
  const message = 'Hello Vue 3'
  const count = ref(0) // reactive variable
  const user = reactive({
    name: 'John Doe',
    age: 30
  })
  // สร้างฟังก์ชัน
  const sayHello = () => {
    alert('Hello ' + user.name)
  }
  const countUp = () => {
    count.value++
  }
  const countDown = () => {
    count.value--
  }
</script>

<template>
  <h1>Vue 3</h1>
  <p>
    <button @click="countDown()">-</button> 
    {{ count }} 
    <button @click="countUp()">+</button>
  </p>
  <p>{{ message }}</p>
  <button @click="sayHello()">Hello</button>
</template>

<style scoped>
  h1 {
    color: red;
  }
  button {
    background-color: blue;
    color: white;
  }
</style>