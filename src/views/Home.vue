<template>
  <div class="home">
    <WalletConnect />
  </div>
</template>

<script>
import WalletConnect from '../components/WalletConnect.vue';

export default {
  components: {
    WalletConnect,
  },
};
</script>

<style scoped>
.home {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 100vh;
  background-color: black;
  color: white;
  text-align: center;
}
</style>
