<script setup lang="ts">
import { useCounter, } from "./stores/counter";

const counter = useCounter()
</script>

<template>
  <p>The counter is at {{ counter.n }}</p>
  <button @click="counter.n++">Increment</button>
  <button @click="counter.n--">Decrement</button>
  <button @click="counter.n = 0">Reset</button>
</template>
