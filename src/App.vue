<template>
  <div class="app">
    <h1>HI</h1>
    <p>{{ name }} - age: {{ age }}</p>
    <button @click="changeName('Jackie Daytona')">change name</button>
    <button @click="changeAge('only known to JD')">change age</button>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'App',
  components: {},
  data() {
    return {
      name: 'Laslo Cravensworth',
      age: 180 as number | string,
    };
  },
  methods: {
    changeName(name: string) {
      this.name = name;
    },
    changeAge(age: number | string) {
      this.age = age;
    },
  },
});
</script>

<style></style>
