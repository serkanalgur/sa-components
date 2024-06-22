<template>
  <button class="personal-button" @click="showAlert">
    {{ props.text }}
  </button>
</template>

<script setup>
  const props = defineProps(["text"]);

  function showAlert() {
    console.log("alert");
  }
</script>

<style scoped>
  .personal-button {
    background-color: #000;
    color: #fff;
    padding: 10px 20px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
  }
</style>
