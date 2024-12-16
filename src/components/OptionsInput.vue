<template>
  <div class="input-wrapper">Options Input: {{ inputValue }}</div>
  <input @input="inputValueChange" :value="inputValue" />
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'OptionsInput',
  data() {
    return {
      inputValue: '',
    };
  },
  methods: {
    inputValueChange($event) {
      this.inputValue = $event.target.value;
    },
  },
});
</script>

<style scoped>
.input-wrapper {
  font-size: 30px;
  color: green;
}
</style>
