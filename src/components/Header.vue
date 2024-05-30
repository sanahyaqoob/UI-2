<template>
  <header>
    <button @click="toggleHelp">Help</button>
    <Help v-if="showHelp" @close="toggleHelp"/>
  </header>
</template>

<script>
import Help from './Help.vue';

export default {
  components: {
    Help,
  },
  data() {
    return {
      showHelp: false,
    };
  },
  methods: {
    toggleHelp() {
      this.showHelp = !this.showHelp;
    },
  },
};
</script>

<style scoped>
header {
  background-color: black;
  color: white;
  width: 100%;
  display: flex;
  justify-content: flex-end;
  padding: 10px;
}
button {
  background-color: green;
  color: white;
  border: none;
  padding: 10px;
  cursor: pointer;
}
</style>
