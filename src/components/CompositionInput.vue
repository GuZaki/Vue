<template>
  <div class="input-wrapper">Composition Input: {{ inputValue }}</div>
  <input @input="inputValue = $event.target.value" :value="inputValue"/>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const inputValue = ref<string>('');
</script>

<style scoped>
.input-wrapper {
    font-size: 30px;
    color: blue;
}
</style>

