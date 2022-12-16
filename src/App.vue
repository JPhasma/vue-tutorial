<template>
  <div class="app">
    <h1>HI</h1>
    <p>{{ name }}</p>
    <button @click="changeName('Jackie Daytona')">change name</button>
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
  },
});
</script>

<style></style>
